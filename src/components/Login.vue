<template>
  <div class="bg">
    <img class="images" src="../assets/giant_text.png"> 
    
<div class="container">
  <input type="text" placeholder="email" class="input">
  <br>
  <input type="password" placeholder="password" class="input">
  <br><br>
  <button type="button" class="button">Log In</button>
</div>
  </div>
</template>

<script lang="ts">
import Vue from "vue"

export default Vue.extend({
  name: "HelloWorld",
  props: {
    msg: String
  }
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 0px 0 0;
}

.images {
  max-width: 40%;

  min-height: 30%;
  height: auto;
  width: auto;
}
ul {
  list-style-type: none;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

p {
  color: black;
  font-size: 100px;
  font-family: ubuntu;
  text-align: center;
  text-shadow: 4px 4px 0 rgba(0, 0, 0, 0.1);
}
.bg {
  background: linear-gradient(45deg, #30496b, #30b8d2);
  flex: 1;
  flex-direction: column;
}
.button {
  background: #009933;
  align-self: flex-end;
  width: 100%;
  max-width: 400px;
  margin: 0 auto;
  border-radius: 20px;
  font-size: 2rem;
  font-family: ubuntu;
  text-align: center;
  text-shadow: 2px 2px 0 rgba(0, 0, 0, 0.1);
  padding: 1.4rem 1rem 1.6rem;
}

input {
  background: rgba(255, 255, 255, 0.5);
  align-self: flex-end;
  width: 100%;
  max-width: 400px;
  padding-bottom: 10;
  margin: 0 auto;
  border-radius: 20px;
  padding: 1.4rem 1rem 1.6rem;
}

.container {
  display: flex;
  flex-direction: column;
  // justify-content: center;
  height: 100vh;
  max-width: 1600px;
  padding: 0 15px;
  margin: 0 auto;
}
</style>
