<template>
    <div>
    <div id="app" class="flex items-center justify-center">
        <div @click="playSound()" class='tegel'>
            <img id="image" src="../assets/placeholder.jpg" alt="test">
            <div id="playbutton"></div>
            <h2 id="subtitle">{{ title }}</h2>
            </div>
     </div>
    </div>
</template>

<script>
export default {
    props: [
        'soundFile',
        'title'
    ],
    data() {
        return {
            myTrack: null,
        }
    },
    methods: {
        playSound(){
            this.myTrack.play()
            this.soundEffect = true
        }
    },
    mounted() {
        this.myTrack = new Audio(this.soundFile)
    }
}
</script>

