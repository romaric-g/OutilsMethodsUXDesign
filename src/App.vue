<template>
  <div id="app">
    <Home/>
    <p>Hello World! 000</p>
  </div>
</template>

<script>
import Home from "./components/home/Home"

export default {
  name: 'app',
  components:  {Home},
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Montserrat:700&display=swap');
@import url('https://fonts.googleapis.com/css?family=Lato:300,700&display=swap');
</style>
