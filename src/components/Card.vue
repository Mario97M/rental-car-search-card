<script>
export default {
  name: "Card"
};
</script>

<template>
  <body>
    <div class="patterns">
      <div class="yellow-pattern"></div>
      <div class="orange-pattern"></div>
    </div>
    <div class="card">
      <h1>Serach for a rental car</h1>
    </div>
  </body>
</template>

<style scoped>
body {
  background-color: #fdf9dc;
  width: 100vw;
  height: 100vh;
}

.yellow-pattern {
  width: 20em;
  height: 25em;
  background-color: #fcdb63;
  position: relative;
  right: 15em;
  border-radius: 70px;
}

.orange-pattern {
  width: 12em;
  height: 18em;
  background-color: #fc9a63;
  position: relative;
  left: 15em;
  border-radius: 70px;
}

.patterns {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
  transform: translateY(-50%);
  top: 50%;
  z-index: 1;
}

.card {
  width: 28em;
  height: 33em;
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
}
</style>
