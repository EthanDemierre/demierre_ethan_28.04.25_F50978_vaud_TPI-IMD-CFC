<template>
<section>
  
  <footer>
   
  <div class="partners-section">
    <div class="global">
      <h3>GLOBAL PARTENERS</h3>
      <div class="logos">
        <a href="#"><img class="global-logo" src="public/img/julius.svg" alt="Julius Bär"></a>
        <a href="#"><img class="global-logo" src="public/img/ap.svg" alt="Audemars Piguet"></a>
      </div>
    </div>
    <div class="main">
      <h3>MAIN PARTNERS</h3>
      <div class="logos">
        <a href="#"><img class="mainlogo" src="public/img/superbock.svg" alt="Super Bock"></a>
        <a href="#"><img class="mainlogo" src="public/img/swisscom.svg" alt="Swisscom"></a>
        <a href="#"><img class="mainlogo" src="public/img/vaudoise.svg" alt="Vaudoise"></a>
      </div>
    </div>
  </div>

  <div class="condition">
      <a href="#">Conditions générales</a>
      <a href="#">Gérer les cookies</a>
  </div>

  <div class="suivre">
  <div class="rs">
    <a href="#"><img src="public/img/instagram.svg" alt="Instagram"></a>
    <a href="#"><img src="public/img/facebook.svg" alt="Facebook"></a>
    <a href="#"><img src="public/img/youtube.svg" alt="YouTube"></a>
    <a href="#"><img src="public/img/tiktok.svg" alt="TikTok"></a>
    <p>SUIVRE LE FESTIVAL</p>
  </div>
  <div class="signature">
    <p>Handcrafted by <strong>DEMIERRE ETHAN</strong></p>
  </div>
</div>
</footer>

</section>

</template>



<style>
footer {
  background-color: #EB37AC;
  color: white;
  width: 100%;
  padding: 5rem 0;
  background-image: url(public/img/noise.jpg);
  background-blend-mode: screen;
  display: flex;
  flex-direction: column;
  gap: 3rem;
}

.partners-section {
  display: flex;
  justify-content: space-between;
  margin: 0 5rem;
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
.main h3 {
  font-size: 14px;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 20px;
}

.logos {
  display: flex;
  gap: 50px;
  align-items: baseline; /* au lieu de center */
}
.condition {
  display: flex;
  justify-content: flex-start;
  gap: 5rem;
  margin: 0 5rem;
}

.condition a {
  text-decoration: none;
  color: white;
}

.suivre {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  margin: 0 5rem;
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
}

.global-logo,
.mainlogo {
  height: 100%;
  max-height: 100px; 
  object-fit: contain;
  vertical-align: middle;
  display: inline-block;
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
  }

  .logos {
    flex-wrap: wrap;
    justify-content: center;
    gap: 2rem;
  }

  .condition {
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    margin: 0;
    text-align: center;
  }

  .suivre {
    margin: 0;
    gap: 1rem;
  }

  .rs {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 0.5rem;
    text-align: center;
  }

  .rs p {
    margin-left: 0;
  }

  .signature {
    justify-content: center;
    text-align: center;
  }
}


@import url("/assets/css/font.css");
</style>