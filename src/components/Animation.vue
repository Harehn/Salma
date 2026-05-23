<template>
  <div class="animation open">
    <h1>So, Making this animation was a pain. You'll have to reload if you want to see it again. Oops</h1>
    <p class="message">You got a cookie!!</p>
    <div class="wrapper open">
        <img id="top" :src="require(`@/assets/present_top.png`)" alt="">
        <img id="bottom" :src="require(`@/assets/present_bottom.png`)" alt="">
    </div>
    <img id="cookie" :src="require(`@/assets/cookie.png`)" alt="<a href='https://pngtree.com/freepng/chocolate-chip-cookie-icon-white-background_20892947.html'>png image from pngtree.com/</a>">
  </div>
</template>

<script>
export default {
  name: 'Animation',
  props: {
    message: String
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.wrapper {
  height:40%;
  width:40%;
  margin:auto;
  /* display:contents; */
  position: relative;
  /* display:flex;
  flex-direction: column; */
}
.animation {
    height:100%;
    width:100%;
    color:white;
    /* font-family: monospace; */
    text-align: center;
    align-content: center;
    /* background-color: crimson; */
    background-image: url('~@/assets/present.jpg');
}
#top {
    /* opacity:0.6; */
    height:50%;
    opacity:0.7;
}
#bottom {
    height:52%;
    opacity:0.7;
}
#cookie {
  height:35%;
  transform: translateX(20%);
  position:absolute;
  /* margin:auto; */
  top: 50%;
  left: 38%;
  opacity:0;
}
.message {
  color:black;
  animation: appear 10s linear 2s 1 forwards;
  font-size: 200%;
  opacity:0;
}

.open>#top {
  animation: tilt 5s linear 2s 1 forwards
}
.open>#bottom {
  animation: fade 5s linear 2s 1 forwards
}
.open>#cookie {
  animation: appear 10s linear 2s 1 forwards
}

@keyframes tilt {
  33% {
    transform: translateY(-40%) translateX(20%) rotate(20deg);
  }
  100% {
    transform: translateY(-40%) translateX(20%) rotate(20deg);
    opacity: 0;
  }  
}
@keyframes fade {
  100%{
    opacity: 0;
  }
}
@keyframes appear {
  20% {opacity:0;}
  50%{
    opacity:1;
  }
  99% {
    opacity:1;
  }
  100% {
    opacity:0;
  }
}

</style>
