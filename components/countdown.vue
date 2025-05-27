<template>
    <div class="countdown">
    <ul>   
      <h1><li><span id="days"></span>Jours</li></h1>
      <h1><li><span id="hours"></span>Heures</li></h1>
      <h1><li><span id="minutes"></span>Minutes</li></h1>
      <h1><li><span id="seconds"></span>Secondes</li></h1>
      <h3><li><span id="texte-countdown"></span>AVANT LE DEBUT  <br>DU FESTIVAL</li></h3>
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

    span {
      font-size: 4rem;
      font-weight: bold;
      line-height: 3rem;      
    }

</style>

<style>
@import url("/assets/css/font.css");
</style>