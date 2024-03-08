<script>
    import gh from '../assets/github.png';
    import con from '../assets/confluence.png';
    import jira from '../assets/at.png';
    import vsc from '../assets/vsc.png';
    import slack from '../assets/slack.png';
    import fig from '../assets/figma.png';
    import sql from '../assets/mysql.png';
    import db from '../assets/mongodb.png';
    import linux from '../assets/linux.png';
    import jenkins from '../assets/jenkins.png';
    export default {
        data() {
            return {
                icons: [
                    {
                        source: gh,
                        title: "Github"
                    },
                    {
                        source: con,
                        title: "Confluence"
                    },
                    {
                        source: jira,
                        title: "Jira"
                    },
                    {
                        source: vsc,
                        title: "VS Code"
                    },
                    {
                        source: slack,
                        title: "Slack"
                    },
                    {
                        source: fig,
                        title: "Figma"
                    },
                    {
                        source: sql,
                        title: "My SQL"
                    },
                    {
                        source: db,
                        title: "Mongo DB"
                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="row row-cols-1 row-cols-md-4 g-3">
        <div v-for="icon in icons" class="col">
            <div  class="card text-center w-auto border-dark">
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