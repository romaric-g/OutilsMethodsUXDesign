<template>
  <div id="app">
    <Home/>
    <Layout/>
  </div>
</template>

<script>
import Home from "./components/home/Home"
import Layout from "./components/content/Layout"

export default {
  name: 'app',
  components:  {Home ,Layout},
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap');
@import url('https://fonts.googleapis.com/css?family=Lato:300,700&display=swap');


    h1, h2, h3 {
        font-family: "Montserrat", sans-serif;
        margin: 10px 0;
    }

    p {
        font-family: "Lato", sans-serif;
    }
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@media screen and (max-width: 900px) {
  body {
    font-size: 14px;
    min-width: 350px;
  }
}
     
</style>
