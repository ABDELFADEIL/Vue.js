<template>
  <div id="app">
    <h1>T-shirts Challenge</h1>
    <hr id="hr1">
    <main id="main">
        <div id="head">
          <sidebar></sidebar>
          <my-images></my-images>
        </div>
          <fadeil></fadeil>
          <!-- <nav-sidebar></nav-sidebar> -->

    </main>
  </div>
</template>

<script>
import myImages from "./components/imagesproducts.vue";
import sidebar from "./components/sidebar.vue";
import fadeil from "./components/fadeil.vue";
// import navsidebar from "./components/NavSidebar/navsidebar";


export default {
  name: 'app',
  components: {
    myImages,
    sidebar,
    fadeil,
    // navsidebar,
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss">

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  // margin-top: 60px;
  // margin-right: 40px;
   margin-left: 40px;  
  // width: 1270px;
  // padding: 50px;
}

h1, h2 {
  font-weight: normal;
}
h1 {
  font-size: 16px;
  font-weight: bold;
  float: left;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
h1 {
  padding: 0px;
  margin: 0px;
}
// #main {
  
// }
#head {
 width: 1200px;
  /* margin: auto; */
  height: auto;
  display: flex;
  padding: 0px; 
}
#hr1 {
  width: 1170px;
  float: left;
}


</style>
