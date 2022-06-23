<template>
  <div class="about">
  <h1>Some words about me</h1>
  <div class="content">
    <img class="aboutImage" src="@/assets/images/person.jpg" />
    <div class="aboutText"> 
      <p class="name">George P. Smith</p>
      <p class="results"> Designer dreamer creator</p>
      <p class="moreText">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum ex sed labore ab impedit asperiores quia! Repudiandae, modi doloribus iure laudantium, aliquam nesciunt quae architecto autem eveniet sapiente facere fugiat.
        Doloremque praesentium iure, autem cum esse, voluptatem iusto, molestias voluptas animi deserunt optio natus accusantium recusandae placeat error officia distinctio in explicabo incidunt eaque aliquid dicta totam saepe? Consectetur, enim.
        Error aspernaturporro culpa praesentium autem libero vel labore, maxime magnam placeat? Placeat voluptatum amet eius iusto aliquam magni laudantium dolorum illum! Fugiat, repellat totam ab qui suscipit beatae ratione temporibus.
      </p>
      <button class="contactButton">Contact me...</button>
    </div>
    
  </div>
  </div>
</template>

<script>

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500;700&display=swap');

  h1::before{
    position: absolute;
    content: "About";
    font-size: 40rem;
    color: rgba(79, 77, 73, 0.05);
    top: -50px;
    left: -60px;
    z-index: -10;
  }
  .about{
    width: 90vw;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
  }
  .content{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    margin-top: 2em;
    padding: .5rem 2rem;
  }

  .aboutImage{
    width: 35%;
    height: fit-content;
    border-radius: 20px;
    margin-right: -4rem;
  }

  .aboutText{
    width: 60%;
    margin-top: 3rem;
    padding: 1rem 1.5rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: left;
    font-size: 1.3rem;
    background:rgba(255, 255, 255, .2);
    border-radius: 10px;
    box-shadow: 0 0 20px rgba(0, 0, 0, .2);
  }

  .name{
    font-family: 'Dancing Script', cursive;
    font-size: 7rem;
    transform: rotateZ(-10deg);
    margin: 1rem 0;
  }

  .results{
    font-size: 2rem;
    margin-left: 40%;
    width: 10ch;
    text-align: center;
    letter-spacing: 1rem;
  }
  .moreText{
    font-size: 1.3rem;
    line-height: 150%;
    margin-top: 2rem;
    padding: 0 3rem;
  }
  .contactButton{
    margin: 0 auto;
    padding: .3rem 3rem;
    background: transparent;
    border: none;
    border-top: 1px solid #f9d14b;
    border-bottom: 1px solid #f9d14b;
  }
  .contactButton:hover{
    border-top: 2px solid #f9d14b;
    border-bottom: 2px solid #f9d14b;
  }
</style>