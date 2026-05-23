<template>
  <div class="letter">
    <p>Happy Birthday Salma!! 🎂</p>
    <p>This was a bit of a rush job but I thought I would just deploy it anyway. You might read this during dinner, at karaoke or maybe the day after. I don't know lol.</p>
    <p>But I hope you enjoy the night!!</p>
  </div>
</template>

<script>
export default {
  name: 'Letter',
  props: {
    message: String
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.letter {
    height:80%;
    width:50%;
    color:black;
    /* font-family: monospace; */
    text-align: center;
    align-content: center;
    margin: auto;
    background-color: rgba(255, 255, 255, 0.4);
    border: 5px dotted grey;
    border-radius: 10px;
    overflow-y: auto;
    backdrop-filter: blur(5px);
}
</style>
