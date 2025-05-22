
import type AddcalendarBtn from './addcalendar-btn.vue';
<template>
 <section>
    <div>
        <h1>Notre Newsletter</h1>
        <h4>Inscris-toi maintenant pour être le premier informé dès que
            les billets seront disponibles.
        </h4>
        <h4><a href="">S'abonner</a></h4>
    </div>

 </section>
</template>

<style scoped>
   
    section {
        display: flex;
        justify-content: flex-start;
        flex-direction: column;
        text-align: left;
        height: 20rem;
        background-color: #2631D9;
       
        
    }
  

    div {
        align-items: center;
        margin-left: 5rem;
        margin-right: 5rem;
        max-width: 50%;
    }

    * {
        text-decoration: none;
        color: white;
    }


</style>