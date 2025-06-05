<template>
<section>
  
  <footer>
    <div class="container">
  <div class="partners-section">
      <div class="global">
       
        <h3>GLOBAL PARTENERS</h3>
        <div class="logos">
          <a href="#"><img class="global-logo" src="/img/julius.svg" alt="Julius Bär"></a>
          <a href="#"><img class="global-logo" src="/img/ap.svg" alt="Audemars Piguet"></a>
        </div>
      </div>
      <div class="main">
        <h3>MAIN PARTNERS</h3>
        <div class="logos">
          <a href="#"><img class="mainlogo superbock" src="/img/superbock.svg" alt="Super Bock"></a>
          <a href="#"><img class="mainlogo" src="/img/swisscom.svg?v=3" alt="Swisscom"></a>
          <a href="#"><img class="mainlogo" src="/img/vaudoise.svg?v=4" alt="Vaudoise"></a>
        </div>
      </div>
  </div>

    <div class="condition">
        <a href="#">Conditions générales</a>
        <a href="#">Gérer les cookies</a>
    </div>

    <div class="suivre">
    <div class="rs">
      <a href="#"><img src="/img/instagram.svg" alt="Instagram"></a>
      <a href="#"><img src="/img/facebook.svg" alt="Facebook"></a>
      <a href="#"><img src="/img/youtube.svg" alt="YouTube"></a>
      <a href="#"><img src="/img/tiktok.svg" alt="TikTok"></a>
      <p>SUIVRE LE FESTIVAL</p>
    </div>
    <div class="signature">
      <p>Handcrafted by <strong>DEMIERRE ETHAN</strong></p>
    </div>
  </div>
</div>
</footer>

</section>

</template>



<style scoped>
footer {
  background-color: #EB37AC;
  color: white;
  width: 100%;
  padding: 5rem 0;
  background-image: url(/img/noise.jpg);
  background-blend-mode: screen;
 
}

.container {

}

.partners-section {
  display: flex;
  justify-content: space-between;
  gap: 2rem;
}

.global, .main {
  flex: 1 1 50%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}



.main {
  flex-direction: column;
}

.global h3,
.main  h3 {
  font-size: 14px;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 20px;
}

.logos {
  display: flex;
  gap: 50px;
  align-items: center; 
}
.condition {
  display: flex;
  justify-content: flex-start;
  gap: 1rem;
  
}

.condition a {
  text-decoration: none;
  color: white;
}

.suivre {
  display: flex;
  flex-direction: column;

}

.rs {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  gap: 1rem;
}

.rs p {
  margin-left: 1rem;
  font-size: 14px;
}

.signature {
  display: flex;
  justify-content: flex-end;
  font-size: 12px;
}

.mainlogo {
  height: 100%; 
  max-height: 50px;
  width: 100%;
}

.superbock {
  max-height: 84px;
  height: 84px;
}

.global-logo {
  height: 100%;
  width: 100%;
}

@media (max-width: 960px) {
  footer {
    padding: 3rem 1.5rem;
    gap: 2rem;
  }

  .partners-section {
    flex-direction: column;
    margin: 0;
    gap: 2rem;
  }

  .global,
  .main {
    width: 100%;
    align-items: center;
    text-align: center;
    padding-bottom: 1rem;
  }



  .condition {
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    margin: 0;
    text-align: center;
    padding: 3rem
    
  }

  .suivre {
    margin: 0;
    gap: 1rem;
  }

  .main > h3 {
      margin: 0px;

    }

  .rs {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 0.5rem;
    text-align: center;
    padding: 1rem
  }

  .rs p {
    margin-left: 0;
  }

  .signature {
    justify-content: center;
    
  }
}


@import url("/assets/css/font.css");
</style>