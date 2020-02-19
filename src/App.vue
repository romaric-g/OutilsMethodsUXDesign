<template>
  <div id="app">
    <Home/>
    <Content/>
    <p>Hello World! 000</p>
    
  </div>
</template>

<script>
import Content from "./components/content/Content"
import Home from "./components/home/Home"

export default {
  name: 'app',
  components:  {Home ,Content},
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss">

</style>
