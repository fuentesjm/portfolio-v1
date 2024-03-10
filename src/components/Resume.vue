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
    <a :href="src" target="_blank" class="btn btn-secondary">Resume</a>
</template>

<style scoped>
a
{
    display: flex;
    justify-content: center;
    width: fit-content;
    margin: 0 auto;
}
</style>