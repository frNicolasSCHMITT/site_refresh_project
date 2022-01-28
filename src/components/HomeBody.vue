<template>
  <div class="home-body-bg">
    <!-- <Rainbow /> -->
    <div class="slide-txt">
      <h2>Who are we ?</h2>
      <p>
        <span class="brand-span">PENNY JUICE </span>
        is the leader in childcare juice !
      </p>
      <h3>
        Penny Juice Products Comply With All Requirements for CACFP, Subsidy,
        and Nutrition Set Forth by the FDA
      </h3>
      <p>
        If you're running a childcare center and want to serve healthy beverages
        to kids every day, order quality juice concentrates from Penny Juice of
        America. Our system is fast and easy to use. Penny Juice greatly reduces
        storage and handling requirements. 1 gallon pre-measured mix pitchers
        available to assure cost control and flavor consistency
      </p>
      <h4 class="rainbow_text_animated">A rainbow of tastes !</h4>
      <p>
        15 flavors available including 7 color free flavors. Each case contains
        6 - ½ gallon bottles of your choice. We’ve designed them especially for
        childcare, daycare, preschool, basp and extended daycare. Get in touch
        with us today!
      </p>
      <div class="btn-placement">
        <ButtonMore />
      </div>
    </div>
  </div>
</template>

<script>
import ButtonMore from "@/components/ButtonMore.vue";

export default {
  name: "HomeBody",
  components: {
    ButtonMore,
  },
};
</script>

<style scoped>
.home-body-bg {
  width: 100vw;
  height: 60vh;
  background-image: url(../assets/img/juice_drinking_kids.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position-y: 50%;
  cursor: help;
}

/* TEXT SLIDE */

.slide-txt {
  background-color: rgba(0, 0, 0, 0.75);
  /* border-radius: 0px 20px 20px 0px; */
  padding: 1%;
  color: #fff;
  text-shadow: -1px -1px 0 #000, 1px -1px 0 #000, -1px 1px 0 #000,
    1px 1px 0 #000;
  text-align: justify;
  display: none;
  width: 50%;
  max-width: 500px;
  height: 100%;

  /* for chrome and safari*/
  -webkit-animation-duration: 1s;
  -webkit-animation-name: slidein;

  /*for firefox*/
  -moz-animation-duration: 1s;
  -moz-animation-name: slidein;

  /* for opera*/
  -o-animation-duration: 1s;
  -o-animation-name: slidein;

  /* Standard syntax*/
  animation-duration: 1s;
  animation-name: slidein;
}

@-webkit-keyframes slidein {
  from {
    width: 0%;
    overflow: hidden;
  }

  to {
    width: 50%;
  }
}

@-moz-keyframes slidein {
  from {
    width: 0%;
    overflow: hidden;
  }

  to {
    width: 50%;
  }
}

@-o-keyframes slidein {
  from {
    width: 0%;
    overflow: hidden;
  }

  to {
    width: 50%;
  }
}

@keyframes slidein {
  from {
    width: 0%;
    overflow: hidden;
  }

  to {
    width: 50%;
  }
}

.home-body-bg:hover .slide-txt {
  display: block;
}

.brand-span {
  font-size: 20px;
  font-weight: bold;
  font-style: italic;
}

.slide-txt h2 {
  font-size: 30px;
  margin-bottom: 10px;
}

.slide-txt h3 {
  font-size: 20px;
  font-style: italic;
  text-decoration: underline;
  padding: 10px;
}

.slide-txt p {
  text-indent: 50px;
  line-height: 1.5;
}

/* RAINBOW TXT */

.rainbow_text_animated {
  background: linear-gradient(
    to right,
    #6666ff,
    #0099ff,
    #00ff00,
    #ff3399,
    #6666ff
  );
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  animation: rainbow_animation 5s ease-in-out infinite;
  background-size: 400% 100%;
  font-size: 30px;
  font-weight: bold;
  text-align: center;
  text-shadow: none;
  margin: 10px 0;
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

.btn-placement{
  display: flex;
  justify-content: center;
  margin-top: 25px;
}

/* TEXT DISPLAY */

.slide-txt p,
.slide-txt h2,
.slide-txt h3 {
  /* for chrome and safari*/
  -webkit-animation-duration: 4s;
  -webkit-animation-name: fadein;

  /*for firefox*/
  -moz-animation-duration: 4s;
  -moz-animation-name: fadein;

  /* for opera*/
  -o-animation-duration: 4s;
  -o-animation-name: fadein;

  /* Standard syntax*/
  animation-duration: 4s;
  animation-name: fadein;
}

@-webkit-keyframes fadein {
  from {
    opacity: 0;
    overflow: hidden;
  }

  to {
    opacity: 1;
  }
}

@-moz-keyframes fadein {
  from {
    opacity: 0;
    overflow: hidden;
  }

  to {
    opacity: 1;
  }
}

@-o-keyframes fadein {
  from {
    opacity: 0;
    overflow: hidden;
  }

  to {
    opacity: 1;
  }
}

@keyframes fadein {
  from {
    opacity: 0;
    overflow: hidden;
  }

  to {
    opacity: 1;
  }
}

</style>
