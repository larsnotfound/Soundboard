<template>
  <h1>Ronalds meest <mark>iconische</mark> uitspraken!</h1>
  <div class= "flex-container">
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi"/>
    <sound-tile :soundFile="vaatwasser" title="Vaatwasser" imageURL="imageURL"/>
    <sound-tile :soundFile="audio" title="Content"/>
    <sound-tile :soundFile="audio" title="Content"/>
    <sound-tile :soundFile="audio" title="Content"/>
    <sound-tile :soundFile="audio" title="Content"/>
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
      audio,
      imageURL: '../assets/placeholder.jpg'
    }
  }
}
</script>