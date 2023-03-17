<template>
    <footer>
        <h3>CONTACT</h3>
        <p>Johanna Karlsson</p> 
        <p>Johannahelenakarlsson@gmail.com</p> 
<div class="link-container">
        <a href="github.com/JohannaKarlsson89" class="iconButton"><i class="i fi-brands-github"></i></a>
        <a href="https://www.linkedin.com/in/johanna-karlsson-021919160/" class="iconButton"><i class="fi fi-brands-linkedin"></i></a>
        </div>
    </footer>
   
</template>

<script>
import { RouterLink, RouterView } from 'vue-router'
export default {
    components: {
        RouterLink
    }
} 

</script>

<style>
 /* FOOTER */
 footer {
  padding: 4%;
  text-align: center;
}
footer h3 {
    margin: 0 0 2% 0;
}
.link-container {
  width: 20%;
  margin: 2% auto;
}
.iconButton i{
  font-size: 1.9em;
} 
.iconButton {
  color: #434853;
  text-decoration: none;
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
}
.iconButton :hover{
  color: #000000;
}
@media (min-width: 490px) {
  /* FOOTER */
.link-container {
    display: flex;
    justify-content: space-evenly;
}}
@media (min-width: 765px) {
    .link-box {
    margin-top: 2%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    }
}
</style>