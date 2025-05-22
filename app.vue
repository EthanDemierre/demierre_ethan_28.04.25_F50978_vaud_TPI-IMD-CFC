<script setup lang="ts">
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
        <a href="#programme">Le programme</a>
        <a href="#billeterie">La billeterie</a>
        <a href="#newsletter">La newsletter</a>
        <a href="#affiche">L'affiche</a>
      </nav>
      <Savethedate></Savethedate>
      <date></date>
      <addcalendar-btn></addcalendar-btn>
      <countdown>
      </countdown>
    </section>
  </header>
</template>
<style>
@import url("/assets/css/style.css");
</style>