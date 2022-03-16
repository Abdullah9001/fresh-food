<template>
  <div id="categories">
    <div class="categories-text">
      <h1>Our <span>Categories</span></h1>
    </div>

    <div class="categories-card">
      <div class="card">
        <img src="pngwing.com.png" />
        <h3>Vegitables</h3>
        <h3 class="light">Up to 30%</h3>
        <div class="button">
          <NuxtLink to="#">Shop Now</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="fruits.png" />
        <h3>Fresh Tomato</h3>
        <h3 class="light">Up to 35%</h3>
        <div class="button">
          <NuxtLink to="#">Shop Now</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="dairy.png" />
        <h3>Fresh Meat</h3>
        <h3 class="light">Up to 30%</h3>
        <div class="button">
          <NuxtLink to="#">Shop Now</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="meatt.png" />
        <h3>Fresh Meat</h3>
        <h3 class="light">Up to 40%</h3>
        <div class="button">
          <NuxtLink to="#">Shop Now</NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
#categories {
  padding-top: 4rem;
}
.categories-text {
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

.categories-card {
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
  margin: 0 6rem 0 6rem;
}

.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 1rem;
  margin: 7px;
  height: 300px;
  width: 220px;
  background-color: white;
  box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
  -webkit-box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
  -moz-box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
}

img {
  height: 150px;
  object-fit: cover;
}

h2 {
  font-size: 1.9rem;
  color: rgb(18, 24, 29);
}

.light {
  color: rgb(78, 76, 76);
  padding: 5px 0 5px 0;
}
li {
  list-style: none;
  display: flex;
  padding: 5px;
}

li img {
  height: 15px;
}
.button {
  padding: 10px;
  border: 2px solid orange;
  border-radius: 5px;
  transition: 0.5s ease-in-out;
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
