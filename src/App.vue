<template>
  <h1>Ronalds meest <mark>iconische</mark> uitspraken!</h1>
  <div class= "flex-container">
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
  </div>
</template>

<script>
 
 import SoundTile from './components/SoundTile.vue'
import audio from './assets/audio.mp3'
export default {
  components: {
    SoundTile,
  },
  data() {
    return {
      audio
    }
  }
}
</script>

<style>

 @import url('https://fonts.googleapis.com/css2?family=Urbanist:wght@400;700&display=swap');

body {
    margin: 80px;
}

h1 {
    font-family: 'Urbanist', sans-serif;
    font-size: 36pt;
    font-weight: 400;
}

mark {
   background: none;
   color: orange;
   font-weight: 900;
}

.tegel {
    max-width: 350px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    background-color: orange;
    display: inline-block;
    padding: 0px;
    border-radius: 10px;
    margin: 40px 0px 0px 0px;
}

#image {
    display: block;
    width: 100%;
    height: auto;
    padding: 0;
    border-radius: 10px 10px 0px 0px;
}

.tegel:hover {
    opacity: 90%;
}

#subtitle {
    color: black;
    font-family: 'Urbanist', sans-serif;
    font-size: 21pt;
    font-weight: 800;
    margin: 20px 20px 40px 20px;
}

#playbutton {
    background-color: white;
    border-radius: 50%;
    width: 100px;
    height: 100px;
    z-index: 1000;
    display: inline-flex;
    margin-left: 20px;
    margin-top: -50px;
}

.flex-container {
    display: flex;
    gap: 40px;
    flex-wrap: wrap-reverse;
}

</style>
