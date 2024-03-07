<script>
    export default {
        data() {
            return {
                links: [
                    {
                        title: "About",
                        url: "#top"
                    },
                    {
                        title: "Projects",
                        url: "#project"
                    },
                    {
                        title: "Resume",
                        url: "#resume"
                    }
                ]
            }
        }
    }
</script>

<template>
    <ul class="nav flex-column">
        <li v-for="link in links" class="nav-item">
            <a class="nav-link" aria-current="page" :href=link.url>{{ link.title }}</a>
        </li>
    </ul>
</template>

<style scoped>
    ul li a
    {
        color: #9FADBD;
        transition: .5s;
    }

    ul li a::before
    {
        background: #EFFAFF;
        transition: .5s;
        transform: scale(.9);
        z-index: -1;
    }

    ul li a:hover::before 
    {
        transform: scale(1.1);
    }

    ul li a:hover 
    {
        color: #EFFAFF;
        text-shadow: 0 0 5px #EFFAFF;
     }
</style>