<template >
  <div class="containers" id="scroll-target">
    <div id="Home" v-bind:class="{ easy: isFixed }">
      <Home/>
    </div>

    <div class="menu" v-bind:class="{ fixed: isFixed }" v-scroll="scrolling">
      <div class="center">
        <div class="inner">
          <button v-scroll-to="'#Home'">Home</button>
          <button v-scroll-to="'#Portfolio'">Portfolio</button>
          <button v-scroll-to="'#Services'">Services</button>
          <button v-scroll-to="'#Tools'">Tools</button>
          <button v-scroll-to="'#Contact'">Contact</button>
        </div>
      </div>
      <div class="smallinner" v-on:click="open_menu">
        <font-awesome-icon icon="bars" class="fa-3x"></font-awesome-icon>
        <div class="smallmenu" v-bind:class=" {visible: isVisible}">
          <div class="smallbutton" v-scroll-to="'#Home'">Home</div>
          <div class="smallbutton" v-scroll-to="'#Portfolio'">Portfolio</div>
          <div class="smallbutton" v-scroll-to="'#Services'">Services</div>
          <div class="smallbutton" v-scroll-to="'#Tools'">Tools</div>
          <div class="smallbutton" v-scroll-to="'#Contact'">Contact</div>
        </div>
      </div>
    </div>

    <div id="Portfolio">
      <Portfolio/>
    </div>
    <div id="Services">
      <Services/>
    </div>
    <div id="Ask">
      <Ask/>
    </div>
    <div id="Tools">
      <Tools/>
    </div>
    <p>
      <a name="Contact"></a>
    </p>
    <div id="Contact">
      <Contact/>
    </div>
  </div>
</template>

<script>
import Home from "./Home";
import Portfolio from "./Portfolio";
import Services from "./Services";
import Tools from "./Tools";
import Contact from "./Contact";
import Ask from "./Ask";
import Vue from "vue";
import VueScrollTo from "vue-scrollto";

Vue.use(VueScrollTo);

export default {
  name: "MainScreen",

  data: () => ({
    isFixed: false,
    isVisible: false
  }),
  methods: {
    scrolling() {
      // let container = document.querySelector("#Home").getBoundingClientRect();
      // let scrollTop = window.pageYOffset || document.documentElement.scrollTop;
      // console.log(container.top);

      let container2 = document.querySelector("#Home").getBoundingClientRect();
      if (container2.bottom <= 0) {
        this.isFixed = true;
      }
      if (container2.bottom > 0) {
        this.isFixed = false;
      }
    },
    open_menu() {
      this.isVisible = !this.isVisible;
    }
  },

  components: {
    Home,
    Portfolio,
    Services,
    Tools,
    Contact,
    Ask
  }
};
</script>

<style>
.menu {
  height: 0;
  bottom: 0;
  left: 0;
  width: 100%;
  margin: 0 auto;
  background-color: #fff;
  /* background-color: white; */
}
.center {
  background-color: #fff;
  width: 100%;
  margin: 0 auto;
}
.isFixed {
  width: 100%;
}
button {
  text-decoration: none;
  outline: none;
  display: inline-block;
  padding: 10px 22px;
  margin: 10px 22px;
  border-radius: 30px;
  background-position: 100% 0;
  background-size: 200% 200%;
  font-size: 24px;
  font-weight: 300;
  color: black;
}
button:hover {
  background-color: lightgray;
}
.fixed {
  position: fixed;

  top: 0;
}

.smallmenu {
  visibility: hidden;
  display: inline-block;
  width:94%
}

.smallbutton {
  text-decoration: none;
  outline: none;
  /* display: block; */
  padding: 5px 11px;
   
 
  background-position: 100% 0;
  background-size: 200% 200%;
  font-size: 20px;
  font-weight: 150;
  color: black;
  /* margin: 0 auto; */
  text-align: center;
  background-color: white;
}

.smallbutton:hover {
  background-color: lightgray;
}
.visible {
  visibility: visible;
}

.containers {
  height: 100%;
  position: relative;
}
html,
body {
  height: 100%;
  font-family: "Arial", Helvetica, sans-serif;
}
#Home {
  height: 90%;
}
h2#portfolio:before {
  background-color: lavender;
  content: "";
  height: 5px;
  width: 100%;
  display: block;

  margin: 5px 0 50px 0;
}
.inner {
  margin: 0 auto;
  width: 840px;
}
.smallinner {
  visibility: hidden;
  z-index: 4;
  background-color: white;

}
.fa-3x {
  color: grey;
 
   
  
}
@media screen and (max-width: 840px) {
  #Home {
    height: auto;
  }

  .center {
    display: none;
  }
  .smallinner {
    visibility: visible;
    width:100%
  }
}
</style>