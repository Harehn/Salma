<template>
  <div class="letter">
    <p>Happy Birthday Johanna!! 🎂</p>
    <p>I made this website to wish you a very happy birthday and to show you thanks for being the best best friend there is. (And also because I am too broke to give you a proper gift, lmao TT). I hope your birthday was amazing despite you being busy with school. What gifts did you receive? Hopefully, they were cooler than this, haha.</p>
    <p>We met a decade ago now, right? We've grown a lot since then. We've spent so much of this friendship far apart but I never feel the distance. I'm glad we are such close friends. Must have to do with our neurospiciness. We've been friends for so long and I wish our friendship lasts forever.</p>
    <p>I want to thank you for always being there for me. I know it can be annoying to put up with me but you have done a good job of it. Despite the distance, your support helps a lot and means a lot to me. Hopefully, I have been able to support you a little bit too. </p>
    <p>Hmm, if this is not gift enough, maybe I can give you something in the campaign. Anyway, enough sappiness. TLDR. Happy Birthday!!</p>
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
