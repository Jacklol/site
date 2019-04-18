<template>
  <div class="Home">
    <div class="centre">
      <!-- <img src='../../image.jpg' alt="альтернативный текст"> -->
      <p>Девиз нашей компании большими буквами</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style scoped>
.Home {
  height: 100%;
  background-image: url("../../image.jpg");
  width: 100%;
  background-size: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.Home p {
  font-size: 80px;
  text-align: center;
  color: white;
}
.centre {
  width: 1140px;
  margin: 0 auto;
}
@media screen and (max-width: 840px) {
 
.Home p {
  font-size: 40px;
  padding: 50px 0;
}

}
</style>