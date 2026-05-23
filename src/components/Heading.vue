<template>
  <div class="heading">
    <div class="content">
      <h1>{{ message }}</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Heading',
  props: {
    message: String
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.heading {
    height:100%;
    width:100%;
    background-image: url('~@/assets/sky.jpg');
    text-align: center;
    align-content: center;
}
.content {
    /* height:100%;
    width:100%; */
    color:white;
    /* font-family: monospace; */
    text-align: center;
    align-content: center;
    font-size: 2em;
    height: fit-content;
    width: fit-content;
    margin: auto;
}
h1 {
    width:30ch;
    text-wrap: nowrap;
    overflow:hidden;
    animation: typing 10s steps(30) infinite alternate-reverse;
}
@keyframes typing {
    0% {
        width:0ch;
    }
    25% {
        width:30ch;
    }
    75% {
        width:30ch;
    }
    100% {
        width:0ch;
    }
}

</style>
