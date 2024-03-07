<script>
    import ss from '../assets/ss.png';
    import se from '../assets/se.png';
    import me from '../assets/me.png';

    export default {
        data() {
            return {
                projects: [
                    {
                        image: ss, 
                        title: "StudySpot",
                        description: `Web App that helps students find study spots including 
                        real-time update for each study spots. The platform provides a seamless
                        solution, offering features such as Wi-Fi and power outlet availability,
                        user ratings, check-in capabilities, search, advanced filtering options,
                        and the ability to submit requests for listing their preferred study spots.`,
                        skills: ["Angular", "HTML", "CSS", "Typescript", "Jenkins", "Flask", "Github", "PostgreSQL", "AWS"],
                        giturl: "https://github.com/ben9543/2023-cecs-senior-project"
                    },
                    {
                        image: se,
                        title: "Search Engine",
                        description: `Python positional index search engine 
                        designed to sift through vast collections of JSON, PDF, 
                        and TXT files. With a simple user interface, users are 
                        prompted to input their query, enabling retrieval of desired 
                        documents. Leveraging advanced indexing techniques, the engine swiftly
                        locates relevant content by analyzing the positional relationship of
                        words within documents, ensuring accurate and efficient search results. Whether you're seeking specific information buried within a myriad of files or exploring diverse textual resources, our search engine offers unparalleled accessibility and precision, empowering users to navigate complex datasets with ease.`,
                        skills: ["Python", "Git"],
                        giturl: "https://github.com/fuentesjm/search-engine"
                    },
                    {   
                        image: me,
                        title: "Portfolio",
                        description: `My portfolio site built with Vue js. Uses bootstrap... 
                        Maybe I'll switch it up to tailwind css. Might develop some game on 
                        here`,
                        skills: ["Vue", "HTML", "CSS", "Javascript", "Bootstrap CSS"],
                        giturl: "https://github.com/fuentesjm/portfolio"
                    }
                ]
            }
        }
    }
</script>

<template>
    <h2>Projects</h2>
    <div v-for="project in projects" class="card border-dark mb-3" style="max-width: 100%;">
        <div class="row g-0">
            <div class="col-md-4" style="margin: auto;"> <!--padding-top: 7%;-->
                <img :src=project.image class="img-fluid rounded-start" alt="Image">
            </div>
            <div class="col-md-8">
                <div class="card-body">
                    <div class="card-header">
                        <h5 class="card-title">{{ project.title }}</h5>
                    </div>
                    <p class="card-text">{{ project.description }}</p>
                    <button 
                        v-for="skill in project.skills" 
                        type="button" 
                        class="btn btn-outline-secondary" 
                        style="--bs-btn-padding-y: .25rem; --bs-btn-padding-x: .5rem; --bs-btn-font-size: .75rem; margin-bottom: 10px;" 
                        disabled>{{ skill }}
                    </button>
                    <br>
                    <a :href=project.giturl class="btn btn-secondary">Github</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.card:hover
{
    background: inherit!important;
    background-color: rgba(255, 255, 255, 0.068)!important;
    backdrop-filter: blur(5px)!important;
    border: 1.7px solid rgba(139, 139, 139, 0.637) !important;
    box-shadow: 4px 5px 4px 3px rgba(144, 144, 144, 0.137)!important;
    opacity: .93 !important;
    overflow: hidden !important;
    transition: all .4s ease 0s !important;
}
</style>
