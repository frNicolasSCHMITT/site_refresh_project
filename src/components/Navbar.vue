<template>
  <nav id="nav">
    <!-- <div class="logo"></div> -->
    <ul>
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
}

.logo {
  background-image: url(../assets/img/pennyjuice_logo.png);
  width: 50px;
  height: 50px;
  background-size: cover;
}

.brand {
  background-image: url(../assets/img/pennyjuice_brand_rainbow.png);
  width: 400px;
  height: 40px;
  background-size: cover;
}


#nav ul {
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
  text-underline-offset: 5px;
}

#nav a.router-link-exact-active {
  color: #64B838;
  text-decoration: underline;
  text-underline-offset: 10px;
}


</style>
