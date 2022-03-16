<template>
  <div id="blogs">
    <div class="blogs-text">
      <h1>Our <span>Blogs</span></h1>
    </div>

    <div class="blogs-card">
      <div class="card">
        <img src="shak1.jpg" />
        <div class="fresh">
          <ul>
            <img src="user.svg" />
            <p>By Angel</p>
          </ul>
          <ul>
            <img src="calender.svg" />
            <p>16 July 2021</p>
          </ul>
        </div>
        <div class="fresh-text">
          <hr />
          <h2>Fresh And Organic Vegitables & Fruits</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non,
            delectus!
          </p>
        </div>
        <div class="bt">
          <div class="button">
            <NuxtLink to="#">Read More</NuxtLink>
          </div>
        </div>
      </div>
      <div class="card">
        <img src="shak2.jpg" />
        <div class="fresh">
          <ul>
            <img src="user.svg" />
            <p>By Golden</p>
          </ul>
          <ul>
            <img src="calender.svg" />
            <p>19 May 2022</p>
          </ul>
        </div>
        <div class="fresh-text">
          <hr />
          <h2>Fresh And Organic All The Fruit</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non,
            delectus!
          </p>
        </div>
        <div class="bt">
          <div class="button">
            <NuxtLink to="#">Read More</NuxtLink>
          </div>
        </div>
      </div>
      <div class="card">
        <img src="shak3.jpg" />
        <div class="fresh">
          <ul>
            <img src="user.svg" />
            <p>By Arshiya</p>
          </ul>
          <ul>
            <img src="calender.svg" />
            <p>26 June 2021</p>
          </ul>
        </div>
        <div class="fresh-text">
          <hr />
          <h2>Fresh And Organic Vegitables</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non,
            delectus!
          </p>
        </div>
        <div class="bt">
          <div class="button">
            <NuxtLink to="#">Read More</NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
#blogs {
  padding: 4rem 0 1rem 0;
}
.blogs-text {
  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
  justify-content: space-around;
  padding-bottom: 2rem;
}
h1 {
  font-size: 2rem;
  color: rgb(18, 24, 29);
}

span {
  clip-path: polygon(100% 25%, 91% 49%, 100% 73%, 0 73%, 9% 47%, 0 25%);
  background-color: orange;
  color: white;
  padding: 40px;
}

.blogs-card {
  display: flex;

  justify-content: center;
}

.card {
  display: flex;
  flex-direction: column;
  margin: 7px;
  height: 480px;
  width: 350px;
  background-color: white;
  box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
  -webkit-box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
  -moz-box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
}

img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  padding-right: 5px;
}

h2 {
  padding: 1rem 0 1rem 0;
  color: rgb(18, 24, 29);
}

p {
  color: rgb(78, 76, 76);
}

.fresh {
  display: flex;
  justify-content: space-between;
  padding: 1rem;
}
ul {
  display: flex;
  text-align: center;
  align-items: center;
}

ul img {
  height: 15px;
  width: 15px;
}
.fresh-text {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  padding: 1rem;
}

.bt {
  display: flex;
  align-items: flex-start;
}

.button {
  align-items: flex-start;
  padding: 10px;
  border: 2px solid orange;
  border-radius: 5px;
  transition: 0.5s ease-in-out;
  margin-left: 1rem;
}

a {
  text-decoration: none;
  font-weight: bold;
  color: rgb(0, 0, 0);
}

.button:hover {
  background: orange;
  color: white;
}
</style>
