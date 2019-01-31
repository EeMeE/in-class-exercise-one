<template>
  <div class="hello">
    <input type="text" name="firstName" v-model="nameInput">
    <div v-bind:class="backgroundClassName"></div>
    <div v-bind:class="backgroundClassName">You have exceeded 50 characters</div>
    <!-- v-on -->
    <button v-on:click="handleClick">Submit</button>
    <!-- v-once -->
    <!-- v-html -->
    <div v-html="anchorTag"></div>
    <!-- v-model -->
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>
<script src="./HelloWorld.js"></script>
<style src="./HelloWorld.css" scoped></style>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
