<template>
  <div class="Portfolio">
    <h2 id="portfolio">PORTFOLIO</h2>
    <p>We invented several solutions to make the world better and our clients happier. Here are the most exciting ones we are proud of</p><br/><br/>
 <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
        <v-flex xs4>
          <div class="item">
            <h4>Money2Game</h4><br/>
            <p>
              Problem: Gamers wanted to buy "gold" without spending a cent. 

Solution: We co-founded our 1st startup - Mining of game currency Online. We have emitted "beardeer" e-coins. User earned e-coins by task execution or mining, then exchanged coins to game gold or rubles. Our wallet was integrated with WMmail tasks stock, dozens of Games, payment aggregators. Additionally we invented a Cryptocurrency miner.

            </p>
          </div>
        </v-flex>
        <v-flex xs4>
          <div class="item">
            <h4>Payday Loans Engine</h4><br/>
            <p>Problem: It took up to one year and significant amount of resources to automate every new Lending Company business process. The task was to improve this process and save company money. 

Solution: We have refactored the existing solution and invented a unified core engine that was customizable in a month with much less effort. As a result company's revenue skyrocketed. Our solution was integrated with major Russian Credit Bureaus.</p>
          </div>
        </v-flex>

        <v-flex xs4>
          <div class="item">
            <h4>Lending in Medicine</h4><br/>
            <p>Problem: Our сlient wanted a top-notch automated lending platform with smart scoring and solid numbers. 

Solution: We developed a high-performance enterprise solution with HIPAA, PCI compliance for financing of expensive medical treatment. To speed up time to market, it is integrated with industry leading SaaS for payments processigns, data validation, call campaigns, BI, bookkeeping etc. </p>
          </div>
        </v-flex>
      </v-layout>
 </v-container>
  </div>
</template>

<script>
export default {
  name: "Portfolio"
};
</script>

<style scoped>

.item {
background-color: #f8f8f8;
padding: 20px;
height: 100%;
}

h4 {
   font-size: 35px;
}

p {
  color: #505050;
  font-size: 20px;
  width: 70%;
  margin-left: auto;
  margin-right: auto;
}

#portfolio {
  font-size: 100px;
  text-align: center;

  font-weight: 700;
  text-transform: uppercase;
  
}

.Portfolio {
  padding-top:80px;
}

h2#portfolio:after {
  background-color: #9c9c9c;
  content: "";
  height: 3px;
  width: 36px;
  display: block;
  margin: 28px auto;
}

@media screen and (max-width: 840px) {
#portfolio {
  font-size: 50px;
  font-weight: 350;
  }

  .Portfolio {
        padding-top: 175px;
  }
}
</style>