<template>
    <div>
    <div id="app" class="flex items-center justify-center">
        <div @click="playSound()" class='tegel'>
            <img id="image" src='../assets/ronald.gif'>
            <div id="playbutton">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z" clip-rule="evenodd" />
            </svg>
            </div>
            <h2 id="subtitle">{{ title }}</h2>
            </div>
     </div>
    </div>
</template>





<script>
export default {
    props: [
        'soundFile',
        'title',
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

