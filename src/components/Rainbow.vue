<template>
  <div class="rainbow-container">
    <figure class="rainbow smooth"></figure>
    <div id="shadowBox">
      <p class="rainbow_text_animated">A rainbow of tastes !</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Rainbow",
};
</script>

<style scoped>

.rainbow-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: transparent;
  width: 300px;
  height: 300px;
  cursor: pointer;
  border-radius: 0 0 20px 0;
}

/* RAINBOW ANIM */

.rainbow {
  width: 300px;
  height: 150px;
  margin: 0px;
  position: relative;
  overflow: hidden;
}

.rainbow.smooth::before {
  content: "";
  position: absolute;
  width: 300px;
  height: 300px;
  filter: hue-rotate(-15deg) contrast(95%);
  opacity: 1;
  border-radius: 50%;
  background: radial-gradient(circle at center, transparent, transparent 90px, #9400D3 90px, #9400D3 90px, #4B0082 99.7959183673px, #0000FF 109.5918367347px, #00FF00 119.387755102px, #FFFF00 129.1836734694px, #FF7F00 138.9795918367px, #FF0000 148.7755102041px);
}
/* .rainbow::after {
  content: "";
  position: absolute;
  transform-origin: 150px 150px;
  width: 300px;
  height: 150px;
  background-color: #1A3256;
  animation: wipe 6s ease-in-out infinite;
} */

/* @keyframes wipe {
  0% {
    transform: rotate(0deg);
  }
  20% {
    transform: rotate(180deg);
  }
  70% {
    transform: rotate(180deg);
  }
  90% {
    transform: rotate(360deg);
  }
  100% {
    transform: rotate(360deg);
  }
} */

/* RAINBOW TXT */
#shadowBox {
    background-color: rgb(0, 0, 0);
    /* Fallback color */
    background-color: rgba(0, 0, 0, 0.75);
    /* Black w/opacity/see-through */
    border: 3px solid black;
    text-align: center;
}

.rainbow_text_animated {
    background: linear-gradient(to right, #6666ff, #0099ff , #00ff00, #ff3399, #6666ff);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    animation: rainbow_animation 3s ease-in-out infinite;
    background-size: 400% 100%;
    font-size: 20px;
    font-weight: bold;
}

@keyframes rainbow_animation {
    0%,100% {
        background-position: 0 0;
    }

    50% {
        background-position: 100% 0;
    }
}

</style>