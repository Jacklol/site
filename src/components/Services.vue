<template>
<div class = "Services"> 
<h2 id="services">SERVICES</h2>
<p>The right technology turns business strategies into results. We deliver domain-specific, fully functional, transformative software solutions that drive your business.</p>
 <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
        <v-flex xs4>
          <div>
            <h2>STARTUP & IDEAS</h2>
            <p>
              Do you have an idea for a new product? We are tech savvy to help you realize it. Experienced working in startup environment - R&D, POCs, demos, launch. We build proof-of-concepts quickly to show the art of the possible to our business and key executives.
              Make it work ,then nice, then fast.
            </p>
          </div>
        </v-flex>
        <v-flex xs4>
          <div>
            <h2>VIRTUAL CTO</h2>
            <p>Our Virtual CTO advicing providers and financial services firms on how to evolve the technologies to address evolutionary issues like scalability, interoperability and data privacy. Prepare detailed technical designs that account for security, resiliency, scalability, maintainability, and performance.</p>
          </div>
        </v-flex>

        <v-flex xs4>
          <div>
            <h2>DEDICATED TEAM</h2>
            <p>Brands who want to move quickly without weeks of paperwork and processes may consider us for Special Projects. Accountable for all phases of development process – analysis, design, construction, testing and implementation. We tend to embrace an agile approach, yet can deliver faster results and provide flexibility.</p>
          </div>
        </v-flex>
        <v-flex xs4>
          <div>
            <h2>FINTECH CONSULTING</h2>
            <p>If you are recognize that fintech will have a significant influence on the industry, but you remains unsure of which technologies to adopt and to what degree - here we are.</p>
          </div>
        </v-flex>
        <v-flex xs4>
          <div>
            <h2>REFACTORING</h2>
            <p>Does you software limits your business grows? We can renovate,refactor and upgrade it to high-performance scalable solution. In-depth experience with Java.</p>
          </div>
        </v-flex>

        <v-flex xs4>
          <div>
            <h2>UNIQUE PROBLEM?</h2>
            <p>Tell us your problem and we will brainstorm for the solution.</p>
          </div>
        </v-flex>
      </v-layout>
    </v-container>

</div>
</template>

<script>
export default {
     name: 'Services',
    
}
</script>

<style scoped>
.Services {
        padding-top:60px;
          color:white; 
          background-color:#2c2c2c;
}

#services {
  font-size: 100px;
  text-align: center;
  margin-bottom: 50px;
}
h2#services:after {
  background-color: #9c9c9c;
  content: "";
  height: 3px;
  width: 36px;
  display: block;
  margin: 28px auto;
}

p {
  color: white;
  font-size: 18px;
  width: 70%;
  margin-left: auto;
  margin-right: auto;
  text-align: center;
}

h2 {
  margin:10px auto;
  font-style:italic;
}

@media screen and (max-width: 840px) {
#services {
  font-size: 50px;
}
}
</style>