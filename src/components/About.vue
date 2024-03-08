<script>
    import LanguageIcon from './LanguageIcon.vue';
    import LibrariesFrameworkIcon from './LibrariesFrameworkIcon.vue';
    import ToolIcon from './ToolIcon.vue';
    export default {
        components: {
    LanguageIcon,
    LibrariesFrameworkIcon,
    ToolIcon
},
        data() {
            return {
                bio1: "Back in 2018, I decided to research different engineering major discipline and tumbled head first into the rabbit hole of coding and web development. Throughout my life, I have always been facisnatied with computers to hacking my own wii. Fast-forward to today, I am a Computer Science graduate at California State University of Long Beach. ",
                bio2: "My main focus these days is building products from random ideas in the shower (the quick rich schemes), grinding leetcode, and learning new languages or framework that might be the evolutionary move. I most enjoy building software in the backend of things (because of my lack of creativity) but I do love to explore the realm of web development and learning new ways to modernize a website.",
                bio3: "In my free time, I've also have been consitently hitting the old gym and breakings PR's when I bulk. I do plan to make an app or a website in the future involving nutrition using Kotlin as my language of choice. When I'm not at the computer or at the gym, I'm usually reading self development and investment books."
            }
        }
    }
</script>

<template>
    <p>{{ bio1 }} <br><br><br> {{ bio2 }} <br><br><br> {{ bio3 }}</p>
    <br><br><br>
    <div class="icons">
        <h2>Programming Languages</h2>
        <LanguageIcon></LanguageIcon>
        <br><br><br>
        <h2>Libraries & Frameworks</h2>
        <LibrariesFrameworkIcon></LibrariesFrameworkIcon>
        <br><br><br>
        <h2>Tools & Platforms</h2>
        <ToolIcon></ToolIcon>
    </div>
    
</template>

<style>
    p {color:#9FADBD}
    h2 {color:#EFFAFF; display: flex; justify-content: center;}
</style>./LanguageIcon.vue