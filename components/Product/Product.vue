<template>
  <div id="product">
    <div class="product-text">
      <h1>Our <span>Products</span></h1>
    </div>

    <div class="product-card">
      <div class="card">
        <img src="broccoli.png" />
        <h3>Fresh Broccoli</h3>
        <h3 class="light">$4.99/--10.99/-</h3>
      <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
        <div class="button">
          <NuxtLink to="#">Add to Cart</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="tomato.png" />
        <h3>Fresh Tomato</h3>
        <h3 class="light">$4.99/--10.99/-</h3>
       <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
        <div class="button">
          <NuxtLink to="#">Add to Cart</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="meat.png" />
        <h3>Fresh Meat</h3>
        <h3 class="light">$4.99/--10.99/-</h3>
       <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
        <div class="button">
          <NuxtLink to="#">Add to Cart</NuxtLink>
        </div>
      </div>
    </div>

    <div class="product-card">
      <div class="card">
        <img src="avocado.png" />
        <h3>Fresh Avocado</h3>
        <h3 class="light">$4.99/--10.99/-</h3>
        <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
        <div class="button">
          <NuxtLink to="#">Add to Cart</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="chicken.png" />
        <h3>Chicken</h3>
        <h3 class="light">$4.99/--10.99/-</h3>
       <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
        <div class="button">
          <NuxtLink to="#">Add to Cart</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="lamon.png" />
        <h3>Fresh Lemon</h3>
        <h3 class="light">$4.99/--10.99/-</h3>
        <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
        <div class="button">
          <NuxtLink to="#">Add to Cart</NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

#product {
  padding-top: 1rem;
}
.product-text {
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

.product-card {
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
  height: 350px;
  width: 280px;
  background-color: white;
  box-shadow: 3px 3px 5px 0px rgba(0,0,0,0.65);
-webkit-box-shadow: 3px 3px 5px 0px rgba(0,0,0,0.65);
-moz-box-shadow: 3px 3px 5px 0px rgba(0,0,0,0.65);
}

img {
  height: 200px;
  object-fit: cover;
}

h2 {
  font-size: 1.9rem;
  color: rgb(18, 24, 29);
}

.light{
  color: rgb(78, 76, 76);
  padding: 5px 0 5px 0;
}
li{
  list-style: none;
  display: flex;
  padding: 5px;
}

li img{
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
