<template>
  <footer>
    <div class="show-footer">
      <span>⬆</span>
      <p>Social & Contact Info</p>
      <span>⬆</span>
    </div>
    <div class="feed-row">
      <div class="feed facebook-feed">
        <FacebookFeed />
      </div>
      <div class="feed twitter-feed">
        <TwitterFeed />
      </div>
      <div class="feed contact">
        <h3>Penny Juice of America</h3>
        <p>915 40th Ave Bettendorf, IA 52722</p>
        <p>pennyjuice@hotmail.com</p>
        <p>Phone: 563-386-1999</p>
        <p>Fax: 563-386-6200</p>
        <img src="https://le-cdn.hibuwebsites.com/767557674d6e4362acfa088c81c84a89/dms3rep/multi/opt/PaymentOpts_01172017-290w.png" alt="payment platforms">
      </div>
    </div>
  </footer>
</template>

<script>

import TwitterFeed from "@/components/TwitterFeed.vue";
import FacebookFeed from "@/components/FacebookFeed.vue";

export default {
  name: "Footer",
  components: {
    TwitterFeed,
    FacebookFeed,
  },
};

</script>

<style scoped>

footer {
  position: fixed;
  bottom: 0;
  z-index: 9;
  height: 50px;
  overflow-y: hidden;
  width: 100vw;
  background-color: blue;
}

footer:hover{
  height: 50vh;
  overflow-y: unset;
}

.show-footer{
  height: 50px;
  color: #fff;
  font-size: 30px;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

.feed-row{
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

.feed{
  height: 400px;
  width: 400px;
  background-color: #fff;
}

.contact{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.contact h3,
.contact p{
  margin-bottom: 20px;
}

@media (max-width: 1200px){
  .feed{
    width: 350px;
  }
}

@media (max-width: 1100px){
  .feed{
    width: 300px;
  }

}

@media (max-width: 1000px){
  footer:hover{
    height: 85vh;
  }
  .feed-row {
    flex-direction: column;
    align-items: space-evenly;
    justify-content: space-evenly;
    height: 90vh;
  }
  .feed{
    margin-top: 10px;
    width: 300px;
    height: 500px;
  }
}

</style>