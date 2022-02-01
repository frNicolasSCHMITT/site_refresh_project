<template>
  <nav id="nav">
    <div class="mobile-mode">
      <div class="mobile-nav">
        <router-link to="/"> <div class="mobile-brand"></div> </router-link>
        <div class="logo"></div>
      </div>
      <ul class="mobile-nav-list">
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/shop">Shop</router-link></li>
      </ul>
    </div>
    <ul class="nav-list">
      <router-link to="/"> <div class="brand"></div> </router-link>
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/about">About</router-link></li>
      <li><router-link to="/shop">Shop</router-link></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>

#nav {
  width: 100%;
  height: 50px;
  display: flex;
  /* border-bottom: black 1px solid; */
  margin-bottom: 5px;
  position: fixed;
  top: 0;
  z-index: 9;
  background-color: #fff;
}

.mobile-mode{
  display: none;
}

.brand {
  background-image: url(../assets/img/pennyjuice_brand_rainbow.png);
  width: 400px;
  height: 40px;
  background-size: cover;
}


.nav-list {
  list-style: none;
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}

#nav a {
  font-weight: bold;
  color: #81511d;
  font-size: 30px;
  text-decoration: transparent;
}

#nav a:hover{
  color: #d39609;
  text-decoration: underline;
  /* text-underline-offset: 5px; */
}

#nav a.router-link-exact-active {
  color: #64B838;
  text-decoration: underline;
  text-underline-offset: 10px;
}

@media (max-width: 769px){
  .brand {
    background-image: url(../assets/img/pennyjuice_brand_rainbow.png);
    width: 300px;
    height: 30px;
    background-size: cover;
  }
}

@media (max-width: 600px){
  .brand {
    background-image: url(../assets/img/pennyjuice_brand_rainbow.png);
    width: 200px;
    height: 20px;
    background-size: cover;
  }
}

@media (max-width: 500px){
  .brand {
    background-image: url(../assets/img/pennyjuice_brand_rainbow.png);
    width: 100px;
    height: 10px;
    background-size: cover;
  }
}

@media (max-width: 426px){
  .mobile-mode{
    display: block;
  }
  .mobile-nav{
    display: flex;
    width: 100vw;
    justify-content: space-around;
    align-items: center;
  }
  .mobile-brand {
    background-image: url(../assets/img/pennyjuice_brand_rainbow.png);
    width: 200px;
    height: 20px;
    background-size: cover;
  }
  #nav {
    margin: 0;
    height: unset;
    flex-direction: column;
    align-items: center;
  }
  .nav-list{
    display: none;
  }
  .mobile-nav-list{
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .mobile-nav-list li{
    padding: 15px 0;
  }
  .mobile-mode{
    overflow-y: hidden;
    height: 50px;
  }
  .logo {
    background-image: url(../assets/img/pennyjuice_logo.png);
    width: 40px;
    margin-top: 5px;
    height: 40px;
    background-size: cover;
  }

  .mobile-mode:hover{
    overflow-y: unset;
    height: 250px;
  }
  
}

</style>
