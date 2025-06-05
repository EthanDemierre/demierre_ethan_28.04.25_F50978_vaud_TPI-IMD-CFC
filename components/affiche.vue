<template>
<section id="affiche" >
  <article class="container">
  <div class="text-affiche">
    <h2>Nouvelle vague numérique</h2>
    <br>
    <p>Le Montreux Jazz Festival propose, pour cette 56ᵉ édition, une recherche graphique plus digitalisée. Cette édition vise un public plus jeune. Un renouveau du festival est en cours. Il se digitalise davantage et laisse plus de place à la jeunesse afin qu’elle puisse se retrouver à Montreux. La vague symbolise une énergie puissante et balayante. Cette nouvelle vague numérique incarne donc une génération forte, créative, remplie de valeurs et connectée.

    L’affiche fusionne l’élément naturel de la vague avec une approche digitale. Elle combine l’art visuel, la musique et les nouvelles technologies artistiques pour créer une expérience visuelle en adéquation avec cette jeunesse. En intégrant ces codes, le festival ne fait pas que rajeunir son image : il évolue vers une nouvelle forme mêlant jeunesse, numérique et diversité.

    </p>

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