
import type AddcalendarBtn from './addcalendar-btn.vue';
<template >
 <section id="newsletter"  class="container"  >
    <div class="news">
        <h1>Notre Newsletter</h1>
        <h4>Inscris-toi maintenant pour être le premier informé dès que
            les billets seront disponibles.
        </h4>
        <a href="#" @click.prevent="showModal = true">S'abonner</a>
        <div v-if="showModal" class="modal-overlay" @click.self="closeModal">
      <div class="modal-content">
        <h2>S’inscrire à  <br> <strong>la Newsletter</strong> </h2>
        <p>Soit informer  par mail et téléphone au moment ou  <br> les places sont en vente et ai la possibilité de remporter 2 entrées de ton choix</p>
        <input type="text" name="rere" id="" placeholder="Ecrit ton email..." required="" />
        <div class="btn">   <sinscrire-btn @click="showModal = false">S'abonner</sinscrire-btn></div>
     
        <hr>
        <a class="abandonner" @click="showModal = false">Abandonner</a>
      </div>
    </div>
    </div>
 </section>
</template>

<style scoped>
   
    section {
        display: flex;
        justify-content: flex-start;
        flex-direction: column;
        text-align: left;
        height: 100%;
        padding-top: 5rem;
        padding-bottom: 5rem;
        background-color: #2631D9;
        
    }
  
    .btn {
        display: flex;
        justify-content: center;
    } 

    div {
        align-items: center;
      
       
    }
.news {

}
    * {
        text-decoration: none;
        color: white;
    }

    .modal-overlay {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
     
    }

    .modal-content {
        background:#EB37AC;
        padding: 3rem;
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
        background-image: url(public/img/noise.jpg) ;
        background-blend-mode:screen ;
    }

    .abandonner  {
    display: flex;
    align-items: center;
    margin-top: 1rem;
    justify-content: space-around;

    }     
    p  {
    display: flex;
    text-align: center;
    padding: 1rem;
    }  

    h2 {
    color: #2631D9;
    line-height: 2rem;
    text-align: center;
    }   

    strong {
    color: #2631D9;
    }

    input {
    width: 100%;
    border: 1px solid #000;
    background: #FFF;
    padding: 1rem;
    margin-bottom: 1rem;
    }

    hr {
    margin-top: 2rem;
    }

@media (max-width: 767px) {

    h1 {
      line-height: 65px;
    }

    a {
      line-height: 65px;
    }

}
@import url("/assets/css/style.css");
</style>


<script >
export default {
  data() {
    return {
      showModal: false
    };
  },
  methods: {
    closeModal() {
      this.showModal = false;
    }
  }
};


</script>