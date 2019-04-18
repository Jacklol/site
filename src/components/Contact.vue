<template>
  <div class="Contact">
    <h2 id="contact">CONTACT</h2>
    <p class="contact">Just drop us a line</p>
    <div class="Contact_Info">
      <div class="home">
            <font-awesome-icon icon="home" class="fa-4x"></font-awesome-icon>
            <p>ADDRESS</p>
      </div>
      <div class="phone">
            <font-awesome-icon icon="phone" class="fa-4x"></font-awesome-icon>
            <p>PHONE</p>
      </div>
      <div class="envelope">
           <font-awesome-icon icon="envelope" class="fa-4x"></font-awesome-icon>
           <p>EMAIL</p>
      </div>

   
         
    </div>
  </div>
</template>

<script>


export default {
  name: "Contact"
};
</script>

<style scoped>
#contact {
  font-size: 100px;
  text-align: center;
  color: white;
  font-weight: 700;
  text-transform: uppercase;
}

p.contact {
  font-size: 30px;
  text-align: center;
  color:white
}

.Contact {
  padding-top: 60px;
  background-color: #2c2c2c;
}

h2#contact:after {
  background-color: white;
  content: "";
  height: 3px;
  width: 36px;
  display: block;
  margin: 28px auto;
}

div.Contact_Info > div {
  width: 250px;
  height: 200px;
  background-color: white;
  background-color: lightgrey;
  margin:20px 50px;
}
div.Contact_Info {
display: flex;
  align-items: center;
  justify-content: center
}

.home, .envelope,.phone {
     flex-direction:column;
    display: flex;
  justify-content: center;
  align-items:center;
}


.fa-4x{
  margin:20px 0;
     color:grey;
}

@media screen and (max-width: 840px) {
#contact {
  font-size: 50px;
  font-weight: 350;
  }
}

</style>