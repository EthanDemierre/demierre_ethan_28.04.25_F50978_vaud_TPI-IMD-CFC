<template>
<section id="affiche" >
  <article class="container">
  <div class="text-affiche">
    <h2>Nouvelle vague digitale</h2>
    <br>
    <p>Montreux Jazz Festival propose pour cette 56ème édition. Une recherche graphique plus digitalisée. Cette édition vise un public plus jeune. Un renouveau du festival a lieu. Il se digitalise plus et laisse plus de place à la jeunesse afin de se retrouver à Montreux. La vague est une énergie puissante qui balaye tout ce qu'elle croise… Cette "nouvelle vague digitale" incarne une génération hyperconnectée, créative et en quête de sens. Elle fusionne les arts visuels numériques, la musique et l’innovation technologique pour créer une expérience sensorielle complète. En intégrant ces codes, le festival ne fait pas que rajeunir son image : il devient un véritable carrefour d'expressions, où la culture se vit autant sur scène qu'à travers les écrans, les installations immersives ou les réseaux sociaux.</p>
    <hr>
  </div>
  <div class="affiche">
    <video  autoplay loop muted src="public/vid/affiche-anim-web3.mp4"></video>
  </div>
</article>
</section>

</template>

<style scoped>
.text-affiche {
  flex: 1;

}

video {
  max-width: 100%;

}

section {
  padding-block: 5rem;


  width: 100%;
  background-color: white;
}
article {
  display: flex;
  justify-content: space-around;
  align-items: center;
  gap: 4rem;
}

p {
  text-justify: inter-word;
}

.affiche {
  flex: 1;
  display: grid;
  place-items: center;

}

hr{ 
  margin-top: 1rem;
  border-top: 1px solid red;
  } 

  @media (max-width: 990px)  {
    section {
      padding-block: 2rem;
    }
    article {flex-direction: column;}
    .affiche {
      height: 50%;
      width: 50%;
    }  
  }

  


@import url("/assets/css/font.css");
</style>