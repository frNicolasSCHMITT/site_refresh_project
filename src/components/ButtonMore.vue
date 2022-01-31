<template>
  <button class="Btn_more">{{ BtnName }}</button>
</template>

<script>

export default {
  name: "ButtonMore",
  props: {
    BtnName: String,
  }
};

</script>

<style scoped>

.Btn_more{
  background-color: #64B838;
  border: solid 3px #fff;
  color: #fff;
  font-size: 30px;
  font-weight: bold;
  text-align: center;
  margin: 10px 0;
  padding: 0 5px;
  border-radius: 5px;
  cursor: pointer;  
}

.Btn_more:hover{
  border: solid 3px rgb(0, 150, 50);
  color: rgb(0, 150, 50);
  background-color: #fff;
}

@keyframes rainbow_animation {
  0%,
  100% {
    background-position: 0 0;
  }

  50% {
    background-position: 100% 0;
  }
}

</style>