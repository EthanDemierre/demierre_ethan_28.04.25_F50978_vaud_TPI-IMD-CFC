<script setup lang="ts">
import type Billeterie from './components/billeterie.vue';

useSeoMeta({
  title: 'Montreux Jazz Festival - Save The Date',
  description: 'description',
  ogTitle: 'MONTREUX JAZZ FESTIVAL ',
  ogImage: 'public/img/logo-mjf.png',
})
</script>
<template>
  <section class="navlg">
    <div class="language container ">
      <h4>FR</h4> 
      <h4>IT</h4> 
      <h4>DE</h4> 
    </div>
  </section>
  <header>
    <video class="background-vid" autoplay muted loop src="/public/vid/backgroud-vid.mp4"></video>
    <section>
      <nav class="container">
        <img class="logo-mjf" src="public/img/logo-mjf.png" alt="LOGO MONTREUX JAZZ">
        <h5><a href="#programme">programme</a></h5>
        <h5><a href="#billeterie">billeterie</a></h5>
        <h5><a href="#newsletter">newsletter</a></h5>
        <h5><a href="#affiche">affiche</a></h5>
      </nav>
      <Savethedate></Savethedate>
      <date></date>
    </section>
    <countdown></countdown>
  </header>
  <billeterie></billeterie>
  <newsletter></newsletter>
  <prog></prog>
  <affiche></affiche>
  <Realfooter></Realfooter>
  
</template>

<style>
@import url("/assets/css/style.css");
@import url("/assets/css/font.css");

* {
  scroll-behavior: smooth;
}


</style>