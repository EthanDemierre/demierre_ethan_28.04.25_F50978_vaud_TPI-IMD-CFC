<template>
    <div class="countdown">
    <ul>   
      <li><span class="count" id="days"></span><span class="count-unit">Jours</span></li>
      <li><span class="count" id="hours"></span><span class="count-unit" >Heures </span></li>
      <li><span class="count" id="minutes"></span><span class="count-unit" >Minutes</span></li>
      <li><span class="count" id="seconds"></span><span class="count-unit" >Secondes</span></li>
      <li><h3><span id="texte-countdown"></span>AVANT LE DEBUT  <br>DU FESTIVAL</h3></li>
    </ul>

  </div>
 
</template>



<script setup >
onMounted(() => {
  const second = 1000,
        minute = second * 60,
        hour = minute * 60,
        day = hour * 24;

  // Date fixe : 6 juillet 2026
  const birthday = "07/06/2026";

  const countDown = new Date(birthday).getTime(),
        x = setInterval(function() {    

          const now = new Date().getTime(),
                distance = countDown - now;

          document.getElementById("days").innerText = Math.floor(distance / day);
          document.getElementById("hours").innerText = Math.floor((distance % day) / hour);
          document.getElementById("minutes").innerText = Math.floor((distance % hour) / minute);
          document.getElementById("seconds").innerText = Math.floor((distance % minute) / second);

          // do something later when date is reached
          if (distance < 0) {
            document.getElementById("headline").innerText = "It's the day!";
            document.getElementById("countdown").style.display = "none";
            document.getElementById("content").style.display = "block";
            clearInterval(x);
          }
        }, 0)
})

</script>

<style scoped>

    div {
        display: inline-flex;
        width: 100%;
        padding: 1.25rem 1rem;
        align-items: center;
        height: 15%;
        gap: 3.9375rem;
        background-color: white;
        position: absolute;
        bottom: 0;
       
        
    }
    ul {
        display: flex;
        flex-grow: 1;
        justify-content: center;
        gap: 8rem ;
        padding: 2rem;
        align-items: center; 

    }

    li {
        
        display: inline-flex;
        flex-direction: column;
        align-items: center;
    

    }

    @media (max-width: 1200px) {
      div {
        position: relative;
        display: block;
        height:auto;
        
          
      }

      ul {
        flex-direction: column;
        gap: 1rem;

      }

      span {
        font-size: 20px;
      }
    }




</style>

<style>
@import url("/assets/css/font.css");
</style>