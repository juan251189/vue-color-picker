<template>
  <div id="app">
    <Header></Header>
    <ColorPicker :colors="colors"></ColorPicker>
  </div>
</template>

<script>
import Header from '@/components/Header';
import ColorPicker from '@/components/ColorPicker';
export default {
  name: 'App',
  components:{
    Header,
    ColorPicker
  },
  data(){
    return{
      colors:["#FFF","#000","#AF1E2D","#00EEAE","#FFCE00"]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
body{
  margin: 0;
  padding: 0;
  background-color: #f3f3f3;
}
</style>
