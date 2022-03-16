<template>
  <div class="footer" style="color: aliceblue">
    <div class="footer-page">
      <div class="footer-box">
        <h3>Papry <img class="logo-i" src="basket-shopping-solid.svg" /></h3>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci,
          quia.
        </p>
        <ul>
          <li><img class="logo-c" src="facebook.svg" /></li>
          <li><img class="logo-c" src="twitter.svg" /></li>
          <li><img class="logo-c" src="instagram.svg" /></li>
          <li><img class="logo-c" src="linkedin.svg" /></li>
        </ul>
        <img class="image" src="pngwing.com.png" />
      </div>

      <div class="footer-box">
        <h3>Contact Us</h3>
        <a><img class="logo" src="phone.svg" />+O1771-334455</a>
        <a><img class="logo" src="phone.svg" />+111-222-333</a>
        <a><img class="logo" src="email.svg" />aj345@gmail.com</a>
        <a><img class="logo" src="location.svg" />Dhaka Sirajganj</a>
      </div>

      <div class="footer-box">
        <h3>Quick Links</h3>
        <NuxtLink to="/"><img class="logo" src="arrow.svg" />Home</NuxtLink>
        <NuxtLink to="#product"
          ><img class="logo" src="arrow.svg" />Product</NuxtLink
        >
        <NuxtLink to="#review"
          ><img class="logo" src="arrow.svg" />Review</NuxtLink
        >
        <NuxtLink to="#blogs"
          ><img class="logo" src="arrow.svg" />Blogs</NuxtLink
        >
        <NuxtLink to="#categories"
          ><img class="logo" src="arrow.svg" />Categories</NuxtLink
        >
        <NuxtLink to="#features"
          ><img class="logo" src="arrow.svg" />Features</NuxtLink
        >
        <NuxtLink to="#dashboard"
          ><img class="logo" src="arrow.svg" />Dashboard</NuxtLink
        >
      </div>

      <div class="footer-box">
        <h3>Contact Us</h3>
        <h4>Subscribe For Latest Update</h4>
        <input type="email" placeholder="Email..." />
        <div class="button">
          <NuxtLink class="btn" to="#">Subscribe</NuxtLink>
        </div>
        <div class="picture">
          <img class="logo-i" src="visa.png" />
          <img class="logo-i" src="visa2.jpg" />
          <img class="logo-i" src="visa3.jpg" />
          <img class="logo-i" src="visa4.png" />
        </div>
      </div>
    </div>
    <br /><br /><br />

    <hr />

    <br /><br />
    <div class="footer-text">
      <p>Created by <span> mr. aj designer</span> | all right reserved</p>
    </div>
  </div>
</template>

//
<script></script>

<style scoped>
.footer {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.footer-page {
  justify-content: center;
  display: flex;
  flex-wrap: wrap;
  padding-top: 3rem;
}

.footer-box {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  width: 280px;
  padding: 10px;
  margin: 5px;
}

.logo-i {
  color: orange;
  height: 25px;
}

p {
  color: rgb(78, 76, 76);
  line-height: 1.5rem;
}

ul {
  display: flex;
  text-align: center;
  list-style: none;
}

li {
  padding: 10px;
  background-color: rgb(228, 222, 222);
  color: black;
  margin-right: 5px;
  width: 15px;
  height: 15px;
  transition: 0.5s ease-in-out;
  cursor: pointer;
}

h4 {
  color: rgb(169, 179, 192);
  padding: 1rem 0 1rem 0;
}

input {
  height: 25px;
  padding: 5px;
  margin-bottom: 1rem;
  border: none;
  border-radius: 5px;
  background-color: rgb(169, 179, 192);
}

.logo-c {
  height: 15px;
  width: 15px;
}

.logo {
  height: 15px;
  width: 15px;
  padding-right: 5px;
}

li:hover {
  background-color: orange;
}

.image {
  height: 120px;
  padding-top: 20px;
  object-fit: contain;
}
.footer-box h3 {
  padding-bottom: 5px;
  color: orange;
  font-family: sans-serif;
}

.footer-box a {
  padding: 5px;
  color: rgb(169, 179, 192);
  transition: 1s ease-in-out;
}

.footer-box .logo {
  margin-right: 10px;
  font-size: 15px;
  color: orange;
  transition: 1s ease-in-out;
}

.footer-box a:hover .logo {
  margin-right: 20px;
  color: orange;
}

a {
  text-decoration: none;
}

.button {
  padding: 10px;
  border: 2px solid orange;
  justify-content: center;
  text-align: center;
  border-radius: 5px;
  transition: 0.5s ease-in-out;
  margin-bottom: 10px;
}

.btn {
  text-decoration: none;
  font-weight: bold;
  color: rgb(0, 0, 0);
}

.button:hover {
  background: orange;
}

.footer-box a:hover {
  color: orange;
}

.footer-text p {
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
  color: black;
  font-weight: bold;
  padding: 1rem;
  font-family: sans-serif;
}

.footer-text span {
  color: orange;
  margin: 0 5px 0 5px;
  text-transform: uppercase;
}
</style>
