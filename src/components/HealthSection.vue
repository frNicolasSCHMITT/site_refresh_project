<template>
  <div class="home-health">
    <div class="home-health-bg"></div>
    <div class="home-health-txt">
      <h2>Healthy Juice Concentrates for All Kids to Enjoy</h2>
      <p>
        We provide a variety of flavors that all kids can enjoy! All the juice
        concentrates that we sell are compliant with the USDA and FDA
        guidelines. You don't need to refrigerate the concentrates before or
        after opening them.
      </p>
      <h3>
        Penny Juice Products Comply With All Requirements for CACFP, Subsidy,
        and Nutrition Set Forth by the FDA
      </h3>
      <div class="btn-placement">
          <router-link to="/shop"><ButtonMore BtnName="See more" /></router-link>
      </div>
      <div class="home-health-label desktop"></div>
    </div>
  </div>
  <div class="home-health-label tablet"></div>
  <img class="home-health-label mobile" src="../assets/img/pennyjuice_label.jpg" alt="">
</template>

<script>

import ButtonMore from "@/components/ButtonMore.vue";

export default {
  name: "HealthSection",
  components: {
    ButtonMore,
  },
};

</script>

import ButtonMore from "@/components/ButtonMore.vue";

export default {
  name: "HealthSection",
  components: {
    ButtonMore,
  },
};

<style scoped>

.home-health {
  display: flex;
  width: 100vw;
  margin: 100px 0;
}

.home-health-bg {
  width: 50%;
  height: 500px;
  background-image: url(../assets/img/healthy_sport_kid.jpg);
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
}

.home-health-label{
  background-image: url(../assets/img/pennyjuice_label.jpg);
  width: 550px;
  height: 300px;
  background-repeat: no-repeat;
}

.home-health-txt{
  width: 50%;
  height: 500px;
  max-width: 550px;
  overflow-y: hidden;
}

.btn-placement{
  margin-left: 200px;
}

.home-health-txt h2,
.home-health-txt h3,
.home-health-txt p{
  margin-bottom: 15px;
}

.home-health-txt h3 {
  font-size: 20px;
  font-style: italic;
  text-decoration: underline;
  padding: 10px;
}

.home-health-txt p {
  text-indent: 50px;
  line-height: 1.5;
}

.tablet,
.mobile {
  display: none;
}

@media (max-width: 1100px){
  .desktop{
    display: none;
  }
  .tablet {
    display: block;
    margin-left: calc((100vw - 550px)/2);
  }
  .home-health-bg {
    width: 49%;
    margin-left: 1%;
  }
  .home-health-txt{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    padding: 0 20px;
  }
  .btn-placement{
    margin-left: 0;
  }
}

@media (max-width: 769px){
  .home-health {
    flex-direction: column-reverse;
    align-items: center;
    margin-top: 50px;
  }
  .home-health-txt{
    width: 100%;
    height: unset;
  }
  .home-health-bg{
    width: 100%;
    display: none;
  }
}

@media (max-width: 600px){
  .tablet{
    display: none;
  }
  .mobile{
    display: block;
    width: 90%;
    height: auto;
    margin: 5%;
    
  }
}
</style>
