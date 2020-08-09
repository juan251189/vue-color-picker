<template>
  <div class="color-picker">
    <div
    class="color"
    v-for="(color,i) in colors" :key="i"
    :style="'background:'+color"
    @click="setColor(color)">

    </div>
  </div>
</template>

<script>
export default{
  name:'color-picker',
  props:['colors'],
  methods:{
    setColor(color){
      this.$emit('setColor',color);
    }
  }
}

</script>

<style media="screen">
  .color-picker{
    display: grid;
    width: 125px;
    margin:15px auto;
    grid-template-columns: repeat(5,25px);

  }
  .color{

    height: 25px
  }
</style>
