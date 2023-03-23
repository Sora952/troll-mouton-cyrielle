<template>
  <img alt="Vue logo" class="img" src="./assets/mouton.jpeg" />
  <div id="t">
    <VueWriter
      :array="arr"
      :typeSpeed="70"
      :iterations="'1'"
      :eraseSpeed="50"
      :delay="1000"
    />
  </div>
</template>

<script>
export default {
  data() {
    return { arr: ["Hello !", "Cyrielle c'est la meilleure.", "Bêêêêêh !"] };
  },
};
</script>

<style>
.typewriter.content *:last-child::after {
  font-size: calc(3em + 20px) !important;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#t {
  width: 120px;
  height: 40px;
  background-color: rgba(240, 240, 240, 0.5);
  position: absolute;
  top: 275px;
  left: 650px;
  border: solid 1px black;
  border-radius: 8px;
  padding: 15px;
}
</style>
