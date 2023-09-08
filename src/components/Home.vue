<script>
export default {
  name: "Home"
};
</script>

<template>
  <div class="wrapper">
    <div class="container">
      <h1>Snap Rent a Car!</h1>
      <h2>Rent a Car in a Snap!</h2>
      <img src="../assets/images/car-home-page.jpg" alt="" />
      <p>
        Welcome to Snap Rent a Car, where we put the 'vroom' in your room to
        roam! Tired of tedious paperwork and long queues just to get behind the
        wheel? Snap those worries away! With our super-easy, click-tastic
        booking process, you'll go from clicking to cruising faster than you can
        say 'road trip!' Choose from our fleet of fabulous, fun, and
        fuel-efficient cars that are so clean, they practically sparkle.
      </p>
      <p>
        But wait, there's more! Not only do we make renting a car as easy as a
        snap, but we also offer unbeatable rates that'll have your wallet doing
        a happy dance. And let's not forget our top-notch customer service—our
        team is always ready to assist you with a smile, 24/7. So why settle for
        less when you can have the best? Snap, Rent, Drive, and let the good
        times roll!
      </p>
      <button @click="$emit('show-card')">Go to Card</button>
    </div>
  </div>
</template>

<style scoped>
* {
  margin: 0;
}
.wrapper {
  background-color: #fdf9dc;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.container {
  font-family: "Merriweather", serif;
  max-width: 40em;
  background-color: white;
  padding: 3em;
  border-radius: 20px;
  text-align: center;
  line-height: 30px;
  margin: 6em 0;
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
}
img {
    margin-bottom: 1em;
    border-radius: 5px;
}

button {
  margin-top: 2em;
  background-color: #fe6f4f;
  border-radius: 5px;
  border: none;
  color: white;
  cursor: pointer;
  font-size: 1.2rem;
  height: 3em;
  width: 50%;
}

h2 {
  margin: 1em 0;
}
</style>
