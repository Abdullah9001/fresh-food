<template>
  <div class="navber">
    <div class="logo">
      <img class="logo-img" src="basket-shopping-solid.svg" />
      <h2>Fresh Food</h2>
    </div>
    <div class="nav">
      <ul>
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="#features">Features</NuxtLink></li>
        <li><NuxtLink to="#product">Product</NuxtLink></li>
        <li><NuxtLink to="#review">Review</NuxtLink></li>
        <li><NuxtLink to="#blogs">Blogs</NuxtLink></li>
        <li><NuxtLink to="#categories">Categories</NuxtLink></li>
        <li><NuxtLink to="/dashboard">Dashboard</NuxtLink></li>
      </ul>
    </div>
    <div class="icon">
      <li><img class="logo-img" src="magnifying-glass-solid.svg" /></li>
      <li><img class="logo-img" src="cart-shopping-solid.svg" /></li>
      <li @click="showModal"><img class="logo-img" src="user-solid.svg" /></li>
    </div>

    <modal
      styles="backgroundColor:#0F0F0F"
      class="modal"
      name="first-modal"
      :min-width="290"
      :max-width="500"
      :max-height="700"
      height="auto"
    >
      <div class="modal-container">
        <div class="modal-btn">
          <li @click="showSignin = !showSignin">Login</li>
          <li @click="showSignin = !showSignin">Signup</li>
        </div>
        <form v-if="showSignin" method="post">
          <div class="imgcontainer">
            <img src="man.png" alt="Avatar" class="avatar" />
          </div>

          <div class="container">
            <label for="uname">Email</label>
            <input
              v-model="email"
              type="email"
              placeholder="Enter Email"
              name="uname"
            />

            <label for="psw">Password</label>
            <input
              type="password"
              placeholder="Enter Password"
              name="psw"
              v-model="password"
              required
            />

            <button @click.prevent="login" type="submit">Login</button>
            <label>
              <input type="checkbox" checked="checked" name="remember" />
              Remember me
            </label>
          </div>

          <div class="container" style="background-color: #f1f1f1">
            <button @click="hideModal" type="button" class="cancelbtn">
              Cancel
            </button>
          </div>
        </form>
        <form v-else>
          <div class="container">
            <h1>Sign Up</h1>
            <p>Please fill in this form to create an account.</p>
            <hr />

            <label for="email">Name</label>
            <input
              type="text"
              placeholder="Enter Name"
              name="Name"
              v-model="name"
              required
            />

            <label for="age">Age</label>
            <input
              type="age"
              placeholder="Enter Age"
              name="Age"
              v-model="age"
              required
            />

            <label for="email">Email</label>
            <input
              type="email"
              placeholder="Enter Email"
              name="email"
              v-model="email"
              required
            />

            <label for="psw">Password</label>
            <input
              type="password"
              placeholder="Enter Password"
              name="psw"
              v-model="password"
              required
            />

            <label for="psw-repeat">Repeat Password</label>
            <input
              type="password"
              placeholder="Repeat Password"
              name="psw-repeat"
              v-model="cPassword"
              required
            />

            <label>
              <input
                type="checkbox"
                checked="checked"
                name="remember"
                v-model="checkbox"
                style="margin-bottom: 15px"
              />
              Remember me
            </label>

            <button @click.prevent="signUp" type="submit">Sign Up</button>

            <div class="clearfix">
              <button @click="hideModal" type="button" class="cancelbtn">
                Cancel
              </button>
            </div>
          </div>
        </form>
      </div>
    </modal>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  data() {
    return {
      showSignin: true,

      name: '',
      age: null,
      email: '',
      checkbox: false,
      password: '',
      cPassword: '',
    }
  },
  methods: {
    showModal() {
      this.$modal.show('first-modal')
    },
    hideModal() {
      this.$modal.hide('first-modal')
    },

    signUp() {
      const formData = {
        name: this.name,
        age: this.age,
        email: this.email,
        password: this.password,
        cPassword: this.cPassword,
        checkbox: this.checkbox,
      }
      axios
        .post(
          `https://identitytoolkit.googleapis.com/v1/accounts:signUp?key=
AIzaSyCW8crYbDHryyxntSz1tp7zMe18sZ5wRp0`,
          {
            email: formData.email,
            password: formData.password,
            returnSecureToken: true,
          }
        )
        .then((res) => console.log(res))
        .catch((res) => console.log(res))
    },
    login() {
      const formData = {
        email: this.email,
        password: this.password,
      }
      axios
        .post(
          `https://identitytoolkit.googleapis.com/v1/accounts:signInWithPassword?key=AIzaSyCW8crYbDHryyxntSz1tp7zMe18sZ5wRp0`,
          {
            email: formData.email,
            password: formData.password,
            returnSecureToken: true,
          }
        )
        .then((res) => console.log(res))
        .catch((res) => console.log(res))
    },
  },
}
</script>

<style scoped>
.navber {
  display: flex;
  justify-content: space-around;
  text-align: center;
  align-items: center;
  padding: 10px;
}

.logo {
  display: flex;
  align-items: center;
  justify-content: center;
  word-spacing: 0;
}
h2 {
  color: rgb(18, 24, 29);
}
h1 {
  color: #f1f1f1;
}
p {
  color: #f1f1f1;
  padding-bottom: 1rem;
}
.logo-img {
  height: 25px;
}

.nav ul {
  display: flex;
  list-style: none;
}

.nav ul li {
  padding: 10px;
  list-style: none;
}
li a {
  font-size: 16px;
  width: 10px;
  color: rgb(78, 76, 76);
  text-decoration: none;
  font-weight: bold;
}

.icon {
  display: flex;
}

.icon li {
  list-style: none;
  cursor: pointer;
}

.icon img {
  font-size: 10px;
  margin: 4px;
  padding: 10px;
  background-color: rgb(228, 222, 222);
  height: 20px;
}

.icon img:hover {
  background-color: orange;
  transition: 0.5s ease-in-out;
}

/* modal form */
form {
  border: 3px solid #f1f1f1;
}

/* Full-width inputs */
input[type='text'],
input[type='password'],
input[type='age'],
input[type='email'] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

.modal-btn {
  display: flex;
  justify-content: space-around;
  padding: 1rem;
}

.modal-btn li {
  list-style: none;
  padding: 0.5rem 1rem;
  color: #f1f1f1;
  background-color: orange;
  cursor: pointer;
}

/* Set a style for all buttons */
button {
  background-color: orange;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}

/* Add a hover effect for buttons */
button:hover {
  opacity: 0.8;
}

/* Extra style for the cancel button (red) */
.cancelbtn {
  width: auto;
  padding: 10px 18px;
  background-color: #f44336;
}

/* Center the avatar image inside this container */
.imgcontainer {
  text-align: center;
  margin: 24px 0 12px 0;
}

/* Avatar image */
img.avatar {
  width: 20%;
  height: 20%;
  object-fit: cover;
  border: 2px solid orange;
}

/* Add padding to containers */
.container {
  padding: 16px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

label {
  color: #f1f1f1;
  font-weight: bold;
  font-size: 1rem;
}

/* The "Forgot password" text */
span.psw {
  float: right;
  padding-top: 16px;
}
</style>
