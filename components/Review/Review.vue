<template>
  <div id="review">
    <div class="review-text">
      <h1>Our <span>Review</span></h1>
    </div>

    <div class="review-card">
      <div class="card">
        <img class="man" src="man1.png" />
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia sint unde molestiae dolorum id! Recusandae perspiciatis id ad molestias deleniti.</p>
        <h3>Jack</h3>
        <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
      </div>
      <div class="card">
        <img class="man" src="man2.png" />
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia sint unde molestiae dolorum id! Recusandae perspiciatis id ad molestias deleniti.</p>
        <h3>Aj</h3>
        <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
      </div>
      <div class="card">
        <img class="man" src="man3.png" />
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia sint unde molestiae dolorum id! Recusandae perspiciatis id ad molestias deleniti.</p>
        <h3>John</h3>
        <li>
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-solid.svg">
          <img src="star-half-stroke-solid.svg">
        </li>
      </div>
    </div>
  </div>
</template>

<style scoped>
#review {
  padding-top: 4rem;
}
.review-text {
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



.review-card {
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
  width: 290px;
  background-color: white;
  box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
  -webkit-box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
  -moz-box-shadow: 3px 3px 5px 0px rgba(0, 0, 0, 0.65);
}

.man {
  height: 100px;
  width: 100px;
  border-radius: 50%;
  border: 1px solid darkgrey;
  object-fit: cover;
}

p {
  font-weight: bold;
  line-height: 1.5rem;
  color: rgb(78, 76, 76);
  padding-bottom: 20px;
  font-size: 15px;
}

h2 {
  font-size: 1.9rem;
  color: rgb(18, 24, 29);
}

.light {
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
