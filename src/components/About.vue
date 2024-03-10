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
                bio1: `My journey started in 2018 when I decided to research different engineering 
                    major disciplines and fell head-first into the expansive rabbit hole of coding
                    and web development. Throughout my life, I have always been fascinated with 
                    computers so much so I would hack personal technologies to see how they functioned.
                    Fast-forward to today, I am now a Computer Science graduate at California State
                    University of Long Beach eager to build on top of the skillset I’ve been developing 
                    since I was young.`,
                bio2: `My main focus these days is creating products originated from ideas in the shower,
                    grinding leetcode, and learning new languages or frameworks that might be the 
                    evolutionary move. Today I most enjoy building software on the backend of things as I
                    feel I’m better with technical aspects of coding compared to the creative. Still, I
                    love exploring the realm of web development and learning new ways to modernize a 
                    website where I can showcase that.`,
                bio3: `As for my hobbies, I’ve also been consistently going to the gym and breaking personal
                    records. I understand that a healthy mind requires a healthy body so I do my best to 
                    maintain both. I do plan to make an app or website in the future involving nutrition 
                    using Kotlin as my language of choice. When I’m not at the computer or the gym, I’m 
                    usually reading self-development and investment books. Even though I have graduated I 
                    understand the importance of the continual education of oneself and building where you 
                    find yourself to be lacking.`
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