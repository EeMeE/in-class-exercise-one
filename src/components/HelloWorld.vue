<template>
  <div class="hello">
    <!-- -->
    <!-- input and line validation flexbox -->
    <div class="input-wrapper">
      <input type="text" v-model="inputValue" v-bind:class="inputValidationClass">
      <!--
        <div v-if="inputValue.length > 50">you exceeded 50 characters</div>
      -->
      <div v-if="inlineValidationClass" class="inline-validation">you exceeded 50 characters</div>
    </div>
    <div class="button-wrapper">
      <button v-bind:disabled="isButtonDisabled">Submit</button>
    </div>

    <!-- v-once -->
    <!-- v-html -->
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
