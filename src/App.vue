<template>
  <h1>Ronalds meest <mark>iconische</mark> uitspraken!</h1>
  <div class= "flex-container">
    <sound-tile :soundFile="audio.mp3" title="Goeiedag eem, moi" imageURL="./placeholder.jpg"/>
    <sound-tile :soundFile="vaatwasser" title="Vaatwasser" imageURL="./vaatwasser.png"/>
    <sound-tile :soundFile="audio" title="Content" imageURL="./gonald.png"/>
    <sound-tile :soundFile="audio" title="Content" imageURL="./verbazing.png"/>
    <sound-tile :soundFile="audio" title="Content" imageURL="./ronnie.png"/>
    <sound-tile :soundFile="audio" title="Content" imageURL="./flower.png"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi" imageURL="./lach.png"/>
    <sound-tile :soundFile="audio" title="Goeiedag eem, moi" imageURL="./hond.png"/>
  </div>
</template>

<script>
 
import SoundTile from './components/SoundTile.vue'
import audio from './components/SoundTile.vue'
export default {
  components: {
    SoundTile,
  },
  data() {
    return {
      audio,
      imageURL: 'imageURL'
    }
  }
}
</script>