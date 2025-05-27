<template>
<section>
  
  <footer>
   
  <div class="partners-section">
    <div class="global">
      <h3>GLOBAL PARTENERS</h3>
      <div class="logos">
        <a href="#"><img src="public/img/julius.svg" alt="Julius Bär"></a>
        <a href="#"><img src="public/img/ap.svg" alt="Audemars Piguet"></a>
      </div>
    </div>
    <div class="main">
      <h3>MAIN PARTNERS</h3>
      <div class="logos">
        <a href="#"><img src="public/img/superbock.svg" alt="Super Bock"></a>
        <a href="#"><img src="public/img/swisscom.svg" alt="Swisscom"></a>
        <a href="#"><img src="public/img/vaudoise.svg" alt="Vaudoise"></a>
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
    padding:5rem 0rem 5rem 0rem;
    background-image: url(public/img/noise.jpg) ;
    background-blend-mode:screen ;
    
    
 
  }
     
  .partners-section {
    display: flex;
    margin-left: 5rem;
    margin-right: 5rem;
  }
  
  .global, .main {
    flex: 1 1 50%;
    display: flex;
   
    
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
    align-items: center;
  }
  
  .condition a {
    text-decoration: none;
    color: white
  }
 
  .condition {
    display: flex;
    margin-left: 5rem;
    margin-right: 5rem;
    gap: 5rem
  }
 
  .rs {
    
    gap:1rem;
    display: flex;
    flex-direction: row-reverse
  
  
  }  
  .suivre {     
  height: 100%;
  margin-left: 5rem;
  margin-right: 5rem;
}

  .signature {
    margin-top: 1rem;
    display: flex;
    flex-direction: row-reverse
  }    

@import url("/assets/css/font.css");
</style>