<template>
  <div>
    <div class="showcase">
      <div class="showcase-text">
        <h2>
          Are You Looking For A <span>Fresh</span> &
          <span>Organic </span>
          <br />
          Froduct?
        </h2>
        <p>Here You Will Find Everything...!!</p>
        <Div class="button">
          <NuxtLink to="#">Shop Now</NuxtLink>
        </Div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.showcase {
  background-image: url('./static/vegetables.jpg');
  background-size: cover;
  height: 350px;
  margin-bottom: 10px;
}
.showcase-text {
  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
  justify-content: center;
  height: 60vh;
}

h2 {
  color: white;
  font-size: 30px;
  line-height: 2rem;
  padding: 10px;
  line-height: 3rem;
}

span {
  color: orange;
}
br{
  padding: 5px;
}

p {
  color: white;
  padding-bottom: 10px;
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
