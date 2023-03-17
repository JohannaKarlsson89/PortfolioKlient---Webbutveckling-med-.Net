<template>
    
<div class="about-box">
    <h1>Webdeveloper and UX-enthusiast</h1>
<article class="about-article">
<img src="../assets/images/johanna.jpg" class="johannaPic" alt="picture of johanna smiling">
<p>Hi there! I'm Johanna a web developer with a passion for crafting clean and functional websites. I specialize in front-end development, with expertise in HTML, CSS, JavaScript, and Vue. I believe in putting the user first and strive to create intuitive and accessible interfaces that de-light and engage. When I'm not coding, you can find me exploring new hiking trails or trying out new recipes in the kitchen.</p>

</article>
<WhatICanDoList />
</div>

</template>

<script>
import WhatICanDoList from "../components/WhatICanDoList.vue";
export default {
  components: {
    WhatICanDoList
  }
}
</script>
<style>

.about-article {
    width: 95%;
    margin: auto auto;
}
.johannaPic {
  border-radius: 99rem;
  border-width: 2px;
  padding: 0.5rem 2.0rem;
  margin: auto;
}
@media (min-width: 560px) {
    .about-article {
    display: flex;
    flex-direction: row;
    align-items: center;
    column-gap: 2em;
    width: 80%;
    }
}


</style>
