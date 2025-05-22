<template>
<section>
  <article>
  <div class="text-affiche">
    <h2>Nouvelle vague digitale</h2>
    <p>consectetur adipiscing elit. Donec eget odio augue. Aenean eget scelerisque nulla. Ut lacinia tempus pharetra. Sed vitae erat ut augue ultricies porttitor quis varius ex. Etiam laoreet congue enim vel bibendum. Maecenas congue ligula id lacus pellentesque tempus. Duis egestas auctor velit, nec feugiat nunc. Duis eu ipsum dictum, pretium diam ut, vulputate risus. Cras tristique turpis mi, et malesuada risus gravida quis.</p>
    <hr>
  </div>
  <div class="affiche">
    <img src="public/img/affiche.png" alt="public/img/affiche.png">
  </div>
</article>
</section>

</template>

<style scoped>
.text-affiche {
  max-width: 33%;
  margin-top: 5rem;

}

section {
  height: 50rem;
  width: 100%;
  background-color: white;
}
article {
  display: flex;
  justify-content: space-around;
  margin-left: 5rem;
  margin-right: 5rem;
}

.affiche {
  margin-top: 5rem;
}

hr{ 
  margin-top: 1rem;
  border-top: 1px solid red;
  } 

</style>

<style>
@import url("/assets/css/font.css");
</style>