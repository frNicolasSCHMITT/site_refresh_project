<template>
  <button class="Btn_more">See more</button>
</template>

<script>

export default {
  name: "ButtonMore",
};

</script>

<style scoped>

.Btn_more{
  background: linear-gradient(
    to right,
    #6666ff,
    #0099ff,
    #00ff00,
    #ff3399,
    #6666ff
  );
  /* -webkit-background-clip: text;
  background-clip: text; */
  color: #fff;
  animation: rainbow_animation 5s ease-in-out infinite;
  background-size: 400% 100%;
  font-size: 30px;
  font-weight: bold;
  text-align: center;
  text-shadow: none;
  margin: 10px 0;
  padding: 0 5px;
  border-radius: 10px;
  cursor: pointer;  
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