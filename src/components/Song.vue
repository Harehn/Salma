<template>
  <div class="song">
    <p><em>On a silly note, you taught us what the actual lyrics of this song meant </em></p>
<iframe width="853" height="480" src="https://www.youtube.com/embed/Tqr52FpLDRU" title="Naza - MMM (Clip Officiel)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
