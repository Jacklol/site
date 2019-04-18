<template>
  <div class="Tools">
    <h2 id="tools">TOOLS</h2>
    <p
      class="tools"
    >The technology we choose depends on the problem we want to solve. Some things are better done in one stack than another.</p>
    <div id="tools">
      <!-- <v-container grid-list-md text-xs-center>
            <v-layout row wrap>
         <v-flex xs4>
          <img src="../../tool1.png" alt>
        </v-flex>
        <v-flex xs4>
          <img src="../../tool2.png" alt>
        </v-flex>
        <v-flex xs4>
          <img src="../../tool3.png" alt>
        </v-flex>

        <v-flex xs4>
          <img src="../../tool4.png" alt>
        </v-flex>
        <v-flex xs4>
          <img src="../../tool5.png" alt>
        </v-flex>
        <v-flex xs4>
          <img src="../../tool6.png" alt>
        </v-flex>

        <v-flex xs4>
          <img src="../../tool7.png" alt>
        </v-flex>
        <v-flex xs4>
          <img src="../../tool8.png" alt>
        </v-flex>
        <v-flex xs4>
          <img src="../../tool9.png" alt>
        </v-flex>
        </v-layout>
      </v-container>-->

      <div class="container">
        <div class="row">
          <div class="col-sm">
            <img src="../../tool1.png" alt>

            <img src="../../tool2.png" alt>

            <img src="../../tool3.png" alt>
          </div>
          <div class="col-sm">
            <img src="../../tool4.png" alt>

            <img src="../../tool5.png" alt>

            <img src="../../tool6.png" alt>
          </div>
          <div class="col-sm">
            <img src="../../tool7.png" alt>

            <img src="../../tool8.png" alt>

            <img src="../../tool9.png" alt>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Tools"
};
</script>

<style scoped>
.Tools {
  padding-top: 60px;
  margin-left: 15%;
  margin-right: 15%;
}
#tools {
  font-size: 100px;
  text-align: center;
  margin-bottom: 50px;
  font-weight: 700;
  text-transform: uppercase;
}

h2#tools:after {
  background-color: #9c9c9c;
  content: "";
  height: 3px;
  width: 36px;
  display: block;
  margin: 28px auto;
}

p.tools {
  font-size: 30px;
  text-align: center;
}

img {
  width: 250px;

  margin: 30px;
}

.images {
  display: inline-block;
}

.row1 {
  display: inline;
}

.row2 {
  display: inline;
}

.row3 {
  display: inline;
}

@media screen and (max-width: 840px) {
#tools {
  font-size: 50px;
  font-weight: 350;
  }
}
</style>