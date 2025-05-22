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
      <addcalendar-btn></addcalendar-btn>
      <countdown>
      </countdown>
    </section>
  </header>
  <billeterie></billeterie>
  <newsletter></newsletter>
  <prog></prog>
  <affiche></affiche>

  <footer>
    <div class="global-parteners"> 
      <h3>Global parteners</h3>
      <a href="https://www.instagram.com/montreuxjazzfestival" target="_blank" rel="noopener">
        <img src="public/img/julius.svg" alt="Instagram" />
      </a>
      <a href="https://www.facebook.com/montreuxjazzfestival" target="_blank" rel="noopener">
        <img src="public/img/ap.svg" alt="Facebook" />
      </a>
    </div>

    <div class="main-parteners"> 
      <h3>Main parteners</h3>
      <a href="https://www.instagram.com/montreuxjazzfestival" target="_blank" rel="noopener">
        <img src="public/img/superbock.svg" alt="Instagram" />
      </a>
      <a href="https://www.facebook.com/montreuxjazzfestival" target="_blank" rel="noopener">
        <img src="public/img/swisscom.svg" alt="Facebook" />
      </a>
      <a href="https://twitter.com/montreuxjazz" target="_blank" rel="noopener">
        <img src="public/img/vaudoise.svg" alt="Twitter" />
      </a>
    </div>
    <div class="footer-social">
      <a href="https://www.instagram.com/montreuxjazzfestival" target="_blank" rel="noopener">
        <img src="public/img/instagram.svg" alt="Instagram" />
      </a>
      <a href="https://www.facebook.com/montreuxjazzfestival" target="_blank" rel="noopener">
        <img src="public/img/facebook.svg" alt="Facebook" />
      </a>
      <a href="https://twitter.com/montreuxjazz" target="_blank" rel="noopener">
        <img src="public/img/twitter.svg" alt="Twitter" />
      </a>
      <a href="https://www.youtube.com/montreuxjazzvideos" target="_blank" rel="noopener">
        <img src="public/img/youtube.svg" alt="YouTube" />
      </a>
    </div>
    <h3>Handcrafted by Demierre Ethan</h3>
  </footer>
</template>

<style>
@import url("/assets/css/style.css");
@import url("/assets/css/font.css");
</style>