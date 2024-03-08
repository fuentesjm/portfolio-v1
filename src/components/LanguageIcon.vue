<script>
    import py from '../assets/python.png';
    import cpp from '../assets/c++.png';
    import r from '../assets/rust.png';
    import js from '../assets/js.png';
    import java from '../assets/java.png';
    import typescript from '../assets/typescript.png';
    import html from '../assets/html.png';
    import css from '../assets/css.png';

    export default {
        data() {
            return {
                icons: [
                    {
                        source: py,
                        title: "Python"
                    },
                    {
                        source: cpp,
                        title: "C++"
                    },
                    {
                        source: java,
                        title: "Java"
                    },
                    {
                        source: typescript,
                        title: "Typescript"
                    },
                    {
                        source: r,
                        title: "Rust"
                    },
                    {
                        source: js,
                        title: "Javascript"
                    },
                    {
                        source: html,
                        title: "HTML"
                    },
                    {
                        source: css,
                        title: "CSS"
                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="row row-cols-1 row-cols-md-4 g-3">
        <div v-for="icon in icons" class="col">
            <div  class="card text-center border-dark">
                <img :src=icon.source class="card-img-top" alt="Python">
                <div class="card-body">
                    <h5 class="card-title">{{ icon.title }}</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.card:hover
{
    background: inherit!important;
    background-color: rgba(255, 255, 255, .3)!important;
    backdrop-filter: blur(5px)!important;
    border: 1.7px solid rgba(139, 139, 139, 0.637) !important;
    box-shadow: 4px 5px 4px 3px rgba(144, 144, 144, 0.137)!important;
    opacity: .93 !important;
    overflow: hidden !important;
    transition: all .4s ease 0s !important;
}

@media (max-width: 1023px)
{
    .col
    {
        width: 15%;
        box-sizing: content-box;
        margin: 0 auto;
        padding-top: 5%;
    }
    .card-title
    {
        white-space: nowrap;
        display: flex;
        justify-content: center;
    }
}
</style>
