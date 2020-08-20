<template>
  <div class="hello">
    <h1>
      <i class="fas fa-bone"></i>
      {{ msg }}
      <i class="fas fa-bone"></i>
    </h1>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
h1 {
  font-family: "Itim", cursive;
}
</style>
