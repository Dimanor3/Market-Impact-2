<template>
  <div id="nav">
    <img class="logo" src="../src/assets/market-impact-2-logo.png">

    <ul class="nav-button">
      <li class="home">
        <router-link to="/">Home</router-link>
      </li>
      <li class="about">
        <router-link :to="{ name: 'About' }">About</router-link>
      </li>
    </ul>
  </div>
    <router-view/>

  <div id="footer">
    <p>Copyright {{ new Date().getFullYear() }}</p>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.logo {
  width: 10%;
  text-align: left;
  display: block;
  transform: rotate(12deg);
  margin: -30px 0px -46px 0px;
}

#nav {
  padding: 30px;
  background: red;
}

ul.nav-button {
  padding: 0px;
  margin: 0;
  list-style-type: none;
  text-align: right;
}

ul.nav-button li {
  display: inline;
  border: 1px solid black;
  padding: 10px 20px;
  font-size: 24px;
  background: white;
}

ul.nav-button li a {
  text-decoration: none;
}

ul.nav-button li a:hover {
  color: blue;
}

ul.nav-button li a.router-link-exact-active {
  color: #42b983;
}

#footer {
  padding: 30px;
  background-color: red;
}

#footer p {
  color: white;
  font-size: 24px;
}
</style>
