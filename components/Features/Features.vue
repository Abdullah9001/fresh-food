<template>
  <div id="features">
    <div class="feature-text">
      <h1>Our <span>Feature</span></h1>
    </div>
    <div class="feature-card">
      <div class="card">
        <img src="pngwing.com (1).png" />
        <h2>Fast Delivery</h2>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Temporibus
          recusandae omnis non, dolorum a facere.
        </p>
        <div class="button">
          <NuxtLink to="#">Read More</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="pngwing.com.png" />
        <h2>Fresh & Organic</h2>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Temporibus
          recusandae omnis non, dolorum a facere.
        </p>
        <div class="button">
          <NuxtLink to="#">Read More</NuxtLink>
        </div>
      </div>
      <div class="card">
        <img src="pngwing.com (2).png" />
        <h2>Easy Payment</h2>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Temporibus
          recusandae omnis non, dolorum a facere.
        </p>
        <div class="button">
          <NuxtLink to="#">Read More</NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

#features {
  height: 90vh;
  padding-top: 1rem;
}
.feature-text {
  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
  justify-content: space-around;
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

.feature-card {
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
  margin: 0 6rem 0 6rem;
  height: 75vh;
}

.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 1rem;
  margin: 7px;
  height: 400px;
  width: 300px;
  border: 2px solid rgba(230, 216, 216, 0.75);
  background-color: white;
  box-shadow: 3px 3px 5px 0px rgba(0,0,0,0.65);
-webkit-box-shadow: 3px 3px 5px 0px rgba(0,0,0,0.65);
-moz-box-shadow: 3px 3px 5px 0px rgba(0,0,0,0.65);
}

img {
  height: 150px;
  object-fit: cover;
}

h2 {
  font-size: 1.9rem;
  color: rgb(18, 24, 29);
  padding-bottom: 20px;
}
p {
  font-weight: bold;
  line-height: 2rem;
  color: rgb(78, 76, 76);
  padding-bottom: 20px;
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
