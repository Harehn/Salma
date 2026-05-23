<template>
  <div class="song">
    <p><em>On a silly note, I keep hearing this song and thinking about you lol. </em></p>
    <iframe src="https://www.youtube.com/embed/9YqecbxSr4A" title="Afro B - Drogba (Joanna) Prod by Team Salut [Official Music Video]" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  </div>
</template>

<script>
export default {
  name: 'Song',
  props: {
    message: String
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.song {
    height:100%;
    width:100%;
    color:white;
    /* font-family: monospace; */
    text-align: center;
    align-content: center;
    background-color: crimson;
}
p {
    font-size: 1em;
    margin-bottom: 10%;
}
iframe {
    height: 40%;
    width: 40%;
    border-radius: 20px;
}
</style>
