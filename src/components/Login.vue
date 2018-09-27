<template>
  <div class="bg">
    <div class="image-container">
      <img class="images" src="../assets/text-rectangle-square.png"> 
    </div>
    
<div class="container main-container">
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
import BootstrapVue from "bootstrap-vue"

Vue.use(BootstrapVue)
import "bootstrap/dist/css/bootstrap.css"
import "bootstrap-vue/dist/bootstrap-vue.css"

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
  max-width: 60%;
  max-height: 60%;
  margin-top: 4rem;
  margin-bottom: 4.5rem;
}

.bg {
  background: linear-gradient(35deg, #00b4db, #336699);
  padding-bottom: 400px;
}

.button {
  background: #009933;
  align-self: flex-end;
  width: 100%;
  max-width: 400px;
  margin: 0 auto;
  border-radius: 20px;
  color: white;
  padding: 5px 0px 5px;
  font-size: 2.4rem;
  font-family: ubuntu;
  text-align: center;
  text-shadow: 2px 2px 0 rgba(29, 10, 10, 0.1);
  border: none;
}

.main-container {
  flex-direction: column;
  flex: 1;
  justify-content: flex-end;
}

input {
  background: rgba(255, 255, 255, 0.5);
  width: 100%;
  color: black;
  font-size: 1.2rem;
  max-width: 400px;
  margin: 0 auto;
  border-radius: 20px;
  padding: 1.4rem 1rem 1.2rem;
  border: none;
}

.container {
  display: flex;
  flex-direction: column;
  max-height: auto;
  max-width: 1600px;
  padding: 10px 15px 300px;
  margin: 0 auto;
}
</style>
