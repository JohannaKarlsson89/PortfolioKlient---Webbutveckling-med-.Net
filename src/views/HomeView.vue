<template>
  <div class="about-box">
<h2>My name is <b>JOHANNA</b> - Webdeveloper and UX-enthusiast</h2>
<div class="link-box">
  <a href="#project-box" class="githubButton">See what I can do</a>
  
  <RouterLink to="/about" class="githubButton">Get to know me</RouterLink>
</div>
  </div>

 
  
  <div class="project-box" id="project-box">
<ProjectsList   
    v-for="item in projectsArr"
    :item="item"
    :key="item.id" />
  </div>
</template>

<script>
import ProjectsList from "../components/ProjectsList.vue";
export default {
  data() {
         return {
             projectsArr:[]
         };
     },
  components: {
    ProjectsList
  },
  methods: {
  //Using AJAX to Fetch projects from database
 async getProjects() {
    //fetch
   const resp = await fetch("http://localhost:5117/api/API", {
     method: "GET",
     headers: {
      Accept: "application/json",
       "Content-type": "application/json",
     },
   });
   const data = await resp.json();
   this.projectsArr = data;
 },
 
 },
   mounted() {
     this.getProjects();
   },
   };


</script>

<style>

.about-box .githubButton {


}

</style>