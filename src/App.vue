<template>
  <div id="app">
    <Home/>
    <Content/>
    <p>Hello World! 000</p>
    <Menu/>
  </div>
</template>

<script>
import Content from "./components/content/Content"
import Home from "./components/home/Home"
import Menu from "./components/menu/Menu"

export default {
  name: 'app',
  components:  {Home ,Content, Menu},
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css?family=Montserrat:700&display=swap');
@import url('https://fonts.googleapis.com/css?family=Lato:300,700&display=swap');


* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
