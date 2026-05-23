<template>
  <div class="box">
    <slot class="content"/>
  </div>
</template>

<script>
export default {
  name: 'Box',
  props: {
    color: String
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.box {
    height:100%;
    width:100%;
    scroll-snap-align: center;
    /* background-color: aqua; */
    color:white;
    text-align: center;
    /* display: flex; */
    align-content: center;
}
</style>
