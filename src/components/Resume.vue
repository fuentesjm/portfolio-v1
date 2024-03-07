<script>
    import VuePdfEmbed from 'vue-pdf-embed';
    import 'vue-pdf-embed/dist/style/index.css'
    import pdf from '../assets/JoseMFuentesResume.pdf'
    export default {
        components: {
            VuePdfEmbed
        },
        data() {
            return {
                src: pdf
            }
        }
    }
</script>

<template>
    <h2>Resume</h2>
    <vue-pdf-embed :source="src" />
    
</template>