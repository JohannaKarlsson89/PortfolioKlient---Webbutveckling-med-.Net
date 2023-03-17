<template>
  
<div class="list">
<h3>WHAT I CAN DO</h3>
<div class="columns-WhatcanIdo">
    <ul class="list-row1">
        <li>HTML</li>
        <li>CSS</li>
        <li>Bootstrap</li>
        <li>JavaScript</li>
        <li>Vue</li>
        <li>PHP</li>
    </ul>
<ul class="list-row2">
        <li>Wordpress</li>
        <li>ASP .NET</li>
        <li>C#</li>
        <li>Laravel</li>
        <li>Node och Express</li>
        <li>Databases</li>
    </ul>
</div></div>
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
.list {
    background: rgb(238,174,202);
    background: radial-gradient(circle, rgba(238,174,202,1) 0%, rgba(148,187,233,1) 100%);
    padding: 4%;
    text-align: center;
    line-height: 2.5em;
    
}
.list ul {
    list-style: none;
}
.columns-WhatcanIdo {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    column-gap: 2em;
}
</style>