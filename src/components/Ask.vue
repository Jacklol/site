<template>
  <div class="Ask">
    <div class="Ask_Us_Now">
      <div class="div_with_text">
        <h1>Does your software limit your business growth?</h1>
        <p>You can get renovated or updated building in line with high-performance scalable solution.</p>
      </div>
      <div class="div_with_button">
        <div class="button" v-scroll-to="'#Contact'">Ask Us Now</div>
      </div>
    </div>
    <v-parallax height="400" :src="require('../../view.jpg')">
      <!-- <v-parallax src="../../view.jpg"> -->
    </v-parallax>
  </div>
</template>

<script>
import Vue from "vue";
import VueScrollTo from "vue-scrollto";

Vue.use(VueScrollTo);

export default {
  name: "Ask"
};
</script>

<style scoped>
.div_with_text {
  height: 300px;
  width: 60%;
  display: inline-block;

}

div > h1 {
  text-align: right;
  padding-top: 100px;
}
div > p {
  margin-top: 20px;
  text-align: right;
  font-size: 16px;
}
.div_with_button {
  width: 40%;

  display: inline-block;
 
}

.button {
  text-decoration: none;
  outline: none;
display: inline-block;
  padding: 10px 22px;
  margin: 10px 50px;
  border-radius: 30px;
  background-position: 100% 0;
  background-size: 200% 200%;
  font-size: 24px;
  font-weight: 300;
  background-color: black;
  color: white;
}

.Ask_Us_Now {
 background-color: aquamarine;
}
</style>