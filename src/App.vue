<template>
  <div id="app">

    <index :scroll="false"></index>
  </div>
</template>

<script>
  import fastclick from 'fastclick'
  import index from "./components/index"
export default {
    components:{index},
  name: 'app',
  data () {
    return {

    }
  },mounted: function () {
    fastclick.attach(this.$el)
  }
}
</script>

<style>
@import "assets/css/base.css";
@import "assets/css/mobile_h5.css";
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;width: 100%;height:100%;
}
</style>
