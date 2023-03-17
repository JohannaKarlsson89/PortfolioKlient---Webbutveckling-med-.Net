<template>
 <div class="card-container">
  <div class="card-body">
    <article>
            <h3 class="card-title">{{ item.projectsName }} </h3>
            <p class="card-text">{{ item.projectDescription }} </p>
          <br>
            <a target="_blank" :href="item.projectUrl" class="githubButton"><i class="i fi-brands-github"></i>  GitHub</a>
    
    </article>
  </div>
  </div>
    </template>
    
    <script>
    export default {
      data() {
    
      },
      props: {
        //Obeject of every item in array from HomeView
        item: Object,
      }
    }
    </script>

    <style>
.card-container {
   
    padding:0.5% 0 0 0;
    margin: 0 0 0 0
} 



</style>
