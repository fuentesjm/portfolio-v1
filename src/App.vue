<script>
  import Intro from './components/Intro.vue';
  import Navbar from './components/Navbar.vue';
  import About from './components/About.vue';
  import SocialIcon from './components/SocialIcon.vue';
  import Project from './components/Project.vue';
  import Resume from './components/Resume.vue';

  export default {
    components: {
      Intro,
      Navbar,
      SocialIcon,
      About,
      Project,
      Resume
    },
  }
</script>

<template>
  <div id="align">
    <div id="left">
      <div id="header-area">
        <Intro></Intro>
      </div>
      <div id="navbar">
        <Navbar></Navbar>
      </div>
      <div id="icons">
        <SocialIcon></SocialIcon>
      </div>
    </div>

    <div id="right">
      <div id="about">
        <About></About>
      </div>
      <div id="project">
        <Project></Project>
      </div>
      <div id="resume">
        <Resume></Resume>
      </div>
    </div>
  </div>
</template>

<style>
  #align
  {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-between;
  }

  #left
  {
    margin-left: 5%;
    padding-top: 5%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: auto;
    height: fit-content;
    position: sticky;
    top: 0;
    margin: 0 auto;
  }

  #right
  {
    right: 0;
    margin-right: 5%;
    padding-top: 5%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: fit-content;
    width: 41%;
    margin: 0 auto;
  }
  
  #header-area 
  {
    width:fit-content/*573px*/;
    height:fit-content;
    margin: 0 auto;
  }
  #navbar
  {
    margin-top: 20%;
    width: fit-content;
    height: fit-content;
  }
  #icons
  {
    margin-top: 50%;
    width: 37%;
  }

  #about
  {
    width:auto;
    height: fit-content;
  }

  #project
  {
    margin-top: 20%;
    width: auto;
    height: fit-content;
  }

  #resume
  {
    margin-top: 20%;
    height: fit-content;
    width: 100%;
  }

  @media (max-width: 1023px) {
    #align
    {
      display: flex;
      align-content: flex-start;
      flex-direction: column;
      padding-left: 5%;
      padding-right: 5%;
    }

    #left
    {
      display: flex;
      position: relative;
      flex-direction: column;
      width: 100%;
    }
    #right
    {
      margin-top: 10%;
      height: fit-content;
      width: auto;
      margin: 0 auto;
    }

    #header-area 
    {
      width:100%/*573px*/;
    }
    #navbar
    {
      /**visibility: hidden;*/
      width: 100%;
      display: flex;
      margin-top: 0%;
    }
    #icons
    {
      margin-top: 0%;
      width: 15%;
    }

  }
  
</style>