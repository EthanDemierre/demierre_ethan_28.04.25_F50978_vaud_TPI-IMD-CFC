<script setup lang="ts">
import type Billeterie from './components/billeterie.vue';

useSeoMeta({
  title: 'My Amazing Site',
  ogTitle: 'My Amazing Site',
  description: 'This is my amazing site, let me tell you all about it.',
  ogDescription: 'This is my amazing site, let me tell you all about it.',
  ogImage: 'https://example.com/image.png',
  twitterCard: 'summary_large_image',
})
</script>
<template>
    <div class="language">
      <h4>FR</h4> 
      <h4>IT</h4> 
      <h4>DE</h4> 
    </div>
  <header>
    <video class="background-vid" autoplay muted loop src="/public/vid/backgroud-vid.mp4"></video>
    <section>
      <nav>
        <img class="logo-mjf" src="public/img/logo-mjf.png" alt="LOGO MONTREUX JAZZ">
        <h5><a href="#programme">Le programme</a></h5>
        <h5> <a href="#billeterie">La billeterie</a></h5>
        <h5><a href="#newsletter">La newsletter</a></h5>
        <h5><a href="#affiche">L'affiche</a></h5>
      </nav>
      <Savethedate></Savethedate>
      <date></date>
      <countdown>
      </countdown>
    </section>
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
</style>