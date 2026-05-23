<template>
  <div class="masonry">
            <h1>We don't have enough pictures.</h1>
    <!-- <p>Hello World</p> -->
     <div class="holder">
        <img id="one" :src="require(`@/assets/memories1.jpg`)" alt="">
        <img :src="require(`@/assets/memories2.jpg`)" alt="">
        <img :src="require(`@/assets/memories3.jpg`)" alt="">
        <img :src="require(`@/assets/memories4.png`)" alt="">
     </div>
  </div>
</template>

<script>
export default {
  name: 'Masonry',
  props: {
    message: String
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.masonry {
    height:100%;
    width:100%;
    color:white;
    /* font-family: monospace; */
    text-align: center;
    align-content: center;
    background-color: crimson;
}
.holder {
    height:70%;
    width:50%;
    border: 5px solid grey;
    margin:auto;
    border-radius: 10px;
    background-color: rgb(238, 153, 170);
    display:grid;
    grid-template-columns: 33% 33% 34%;
    grid-template-rows: 33% 33% 34%;
    /* grid-gap: 10px; */
}
img {
    height:96.5%;
    width:96.5%;
    margin:auto;
    /* border: 0.5px solid grey; */
    border-radius: 5px;;
}
#one {
    grid-column: 1 / span 3;
    grid-row: 1 / span 2;
    width:98%;
}
</style>