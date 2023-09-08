<script>
import { Icon } from "@iconify/vue";

export default {
  name: "Card",
  components: {
    Icon
  }
};
</script>

<template>
  <body>
    <div class="patterns">
      <div class="yellow-pattern"></div>
      <div class="orange-pattern"></div>
    </div>
    <div class="card">
      <!-- Pickup location -->
      <h1>Search for a rental car</h1>
      <span>Pick up location</span>
      <div class="pickup-location-input">
        <input placeholder="City, airport, region, district..." type="text" />
      </div>
      <p>
        <label class="checkbox-label">
          <input type="checkbox" class="checkbox" /><span
            class="custom-checkbox"
          ></span>
        </label>
        Deliver the car somewhere else
      </p>
      <!-- Delivery pickup time -->
      <div class="pickup-and-delivery">
        <div class="pickup-and-delivery-left">
          <span>Date of pickup</span>
          <div><input type="date" /></div>
          <div><input type="time" /></div>
        </div>
        <div class="pickup-and-delivery-right">
          <span>Date of delivery</span>
          <div><input type="date" /></div>
          <div><input type="time" /></div>
        </div>
      </div>

      <!-- Age of driver -->

      <p>
        <label class="checkbox-label">
          <input type="checkbox" class="checkbox" /><span
            class="custom-checkbox"
          ></span>
        </label>
        The driver's age between 30 and 65?<Icon
          width="20"
          class="icon-exclamation"
          icon="tabler:exclamation-circle"
          :verticalFlip="true"
        />
      </p>

      <p>
        <Icon
          class="icon-check"
          width="20"
          icon="fluent:checkmark-12-regular"
        />No credit card fees
      </p>

      <p>
        <Icon
          class="icon-check"
          width="20"
          icon="fluent:checkmark-12-regular"
        />No change fees
      </p>

      <p>
        <Icon
          class="icon-check"
          width="20"
          icon="fluent:checkmark-12-regular"
        />Price match guaruntee
      </p>

      <!-- Search button -->

      <a href="#"
        ><div class="search-button"><button>Search</button></div></a
      >
      <div class="go-home-button">
        <button @click="$emit('show-home')">Back to Home</button>
      </div>
    </div>
  </body>
</template>

<style scoped>
body {
  background-color: #fdf9dc;
  height: 100vh;
  width: 100vw;
}

/* Background patterns */

.yellow-pattern {
  background-color: #fcdb63;
  border-radius: 70px;
  height: 25em;
  position: relative;
  right: 15em;
  width: 20em;
}

.orange-pattern {
  background-color: #fc9a63;
  border-radius: 70px;
  height: 18em;
  left: 15em;
  position: relative;
  width: 12em;
}

.patterns {
  align-items: center;
  display: flex;
  flex-direction: column;
  position: relative;
  top: 50%;
  transform: translateY(-50%);
  z-index: 1;
}

.card {
  width: 28em;
  height: 38em;
  background-color: white;
  z-index: 99;
  position: relative;
  margin: auto;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  font-family: "Merriweather", serif;
  padding: 2em;
  border-radius: 2em;
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
}

.card span {
  font-size: 0.7rem;
}

/* Pickup location section */

.pickup-location-input input {
  height: 2em;
  width: 100%;
}

input {
  border: solid 1.2px #8f9dce;
  border-radius: 3px;
}

.pickup-location-input input:focus {
  outline: none;
}

.card p {
  font-size: 0.9rem;
}

/* Pickup time and delivery */

.pickup-and-delivery {
  display: flex;
  gap: 1em;
  justify-content: space-between;
}

.pickup-and-delivery div {
  width: 100%;
}
.pickup-and-delivery input {
  height: 2em;
  width: 100%;
}

.pickup-and-delivery input[type="time"] {
  margin-top: 0.8em;
}

.pickup-and-delivery input:focus {
  outline: none;
}

.search-button button {
  background-color: #fe6f4f;
  border-radius: 15px;
  border: none;
  color: white;
  cursor: pointer;
  font-size: 1.2rem;
  height: 4em;
  width: 100%;
}

/* Icon positioning */

.checbox {
  background-color: blue;
  width: 3em;
}

.icon-check {
  position: relative;
  right: 5px;
  top: 4px;
}

.icon-exclamation {
  left: 5px;
  position: relative;
  top: 4px;
}

.go-home-button {
  text-align: center;
  margin: 2em auto;
}

.go-home-button button {
  background-color: #fe6f4f;
  border-radius: 5px;
  border: none;
  color: white;
  cursor: pointer;
  font-size: 1.2rem;
  height: 3em;
  width: 50%;
  display: inline-block;
}
</style>
