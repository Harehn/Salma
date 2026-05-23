<template>
  <div class="main">    
    <Box style="background-color:grey"><Animation/></Box>
    <Box style="background-color:aqua"><Heading message="Happy birthday, Johanna!! 🎂"/></Box>
    <!-- <Box style="background-color:grey"><Animation/></Box> -->
    <Box style="background-color:blue" id="letter"><Letter/></Box>
    <!-- <Box style="background-color:black">Text Message</Box> -->
    <Box style="background-color:red"><Masonry/></Box>
    <Box style="background-color:purple"><Song/></Box>
  </div>
</template>

<script>
import Box from './components/Box.vue';
import HelloWorld from './components/HelloWorld.vue'
import Heading from './components/Heading.vue'
import Letter from './components/Letter.vue'
import Song from './components/Song.vue'
import Animation from './components/Animation.vue'
import Masonry from './components/Masonry.vue';
//Happy birthday, Johanna!! 🎂
export default {
  name: 'App',
  components: {
    HelloWorld,
    Box,
    Heading,
    Letter,
    Song,
    Animation,
    Masonry
  }
}
</script>


<style>
html, body {
  height:100%;
  width: 100%;
  margin: 0px;
  padding: 0px;
  overflow-x: hidden; 

  /* margin: 0;
  display:flex;
  flex-direction: column;
  justify-content: space-between; */
}
#app {
  height:100%;
  width: 100%;
  margin: 0;
  padding: 0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* scroll-snap-type: y mandatory; */
  /* margin-top: 60px; */
}.main > div {
  scroll-snap-align: start;
}
.main {
  height:100%;
  width: 100%;
  scroll-snap-type: y mandatory;
  overflow-y:scroll;
}
h1 {
  color:black;
}

#letter {
  background-image: url('~@/assets/paper2.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}

/* #letter {
  background-image: url(${require('@/assets/path/to/your/img.jpg')});
} */
</style>
