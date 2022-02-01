<template>
  <div class="about-body">
    <div class="bloc-about">
      <div class="about-img">
        <img src="../assets/img/fruits_juice.jpg" alt="" />
      </div>
      <div class="about-txt">
        <h2>Premium Quality 100% Fruit Juice Concentrate. No Sugar Added. Non Refrigerated</h2>
        <p>Get delicious and nutritious 100% fruit juice from Penny Juice of America. We provide 100% blended fruit juice concentrates that are specially made for kids and meet all the requirements of the FDA with regard to subsidy and nutrition. Customers prefer our products for their benefits, features, variety, service, and competitive pricing.</p>
        <p>These blended fruit juice concentrates are for all childcare centers and preschools. Penny Juice of America uses only the highest quality fruit juice products.</p>
      </div>
    </div>
    <div class="bloc-about bloc-reverse">
      <div class="about-img img-flex">
        <img src="../assets/img/juice_containers.jpg" alt="" />
        <img src="../assets/img/pack_juice.jpg" alt="" />
      </div>
      <div class="about-txt">
        <h3>Easy-To-Make Juice Concentrates</h3>
        <p>Prepare all flavors using seven parts water and one part juice concentrate. You don’t need to refrigerate the concentrate before or after opening it.</p>
        <p>Reduce cost per ounce, storage and handling requirements. </p>
        <h3>Get Juice Concentrates in a Variety of Flavors</h3>
        <p>Kids love penny juice concentrates because it’s available in various exciting flavors and colors. Each case contains six half-gallon bottles of different flavors.</p>
        <p>
          <ul>
            <li>No contracts</li>
            <li>Free delivery nationwide</li>
            <li>Minimum order 1 case</li>
          </ul>
        </p>
        <div class="btn-placement">
          <router-link to="/shop"><ButtonMore BtnName="See more" /></router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ButtonMore from "@/components/ButtonMore.vue";

export default {
  name: "AboutBody",
  components: {
    ButtonMore,
  },
};
</script>

<style scoped>

.about-body {
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100vw;
  height: 100vh;
}

.bloc-about{
  display: flex;
  margin-top: 100px;
}

.bloc-reverse{
  flex-direction: row-reverse;
}

.img-flex{
  display: flex;
  flex-direction: column;
}

.about-img{
  height: 300px;
  width: 550px;
  overflow: hidden;
}

.about-txt{
  width: 50vw;
  padding: 0 5%;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}

</style>
