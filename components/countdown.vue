<template>
    <div class="countdown">
    <ul>   
      <h1><li><span id="days"></span>Jours</li></h1>
      <h1><li><span id="hours"></span>Heures</li></h1>
      <h1><li><span id="minutes"></span>Minutes</li></h1>
      <h1><li><span id="seconds"></span>Secondes</li></h1>
      <h3><li><span id="texte-countdown"></span>AVANT LE DEBUT DU FESTIVAL</li></h3>
    </ul>
    
  </div>
 
</template>



<script setup >
onMounted(() => {
    const second = 1000,
        minute = second * 60,
        hour = minute * 60,
        day = hour * 24;

  //I'm adding this section so I don't have to keep updating this pen every year :-)
  //remove this if you don't need it
  let today = new Date(),
      dd = String(today.getDate()).padStart(2, "0"),
      mm = String(today.getMonth() + 1).padStart(2, "0"),
      yyyy = today.getFullYear(),
      nextYear = yyyy + 1,
      dayMonth = "09/30/",
      birthday = dayMonth + yyyy;
  
  today = mm + "/" + dd + "/" + yyyy;
  if (today > birthday) {
    birthday = dayMonth + nextYear;
  }
  //end
  
  const countDown = new Date(birthday).getTime(),
      x = setInterval(function() {    

        const now = new Date().getTime(),
              distance = countDown - now;

        document.getElementById("days").innerText = Math.floor(distance / (day)),
          document.getElementById("hours").innerText = Math.floor((distance % (day)) / (hour)),
          document.getElementById("minutes").innerText = Math.floor((distance % (hour)) / (minute)),
          document.getElementById("seconds").innerText = Math.floor((distance % (minute)) / second);

        //do something later when date is reached
        if (distance < 0) {
          document.getElementById("headline").innerText = "It's my birthday!";
          document.getElementById("countdown").style.display = "none";
          document.getElementById("content").style.display = "block";
          clearInterval(x);
        }
        //seconds
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

</style>

<style>
@import url("/assets/css/font.css");
</style>