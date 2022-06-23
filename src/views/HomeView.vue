<template>
  <div class="home">
    <div class="header">
      <div class="headerText">
        <h1>This is the best header text. It is explaining everything</h1>
        <h3 class="headerInfo">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda laudantium similique deleniti sunt eum, voluptates culpa, accusantium, corrupti in consequatur officiis officia ea aperiam sequi aliquam earum ullam animi tempore.
        Consequatur nisi, tempore, quia libero nesciunt, esse culpa impedit laboriosam quae porro animi fugiat ducimus possimus alias atque quas eum ratione. Unde, consequuntur nostrum ducimus voluptatibus debitis quibusdam deleniti necessitatibus.
        </h3>
      </div>
      <div class="headerImage">
        <img src="../assets/images/headerPerson02.png" />
        <div class="info">
          <!-- <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
          <path fill="#FF0066" d="M28.7,-32.7C37.8,-26.5,46.5,-18.1,52.2,-6.1C58,5.8,60.9,21.3,54.4,30.2C47.8,39.1,31.8,41.3,20.5,37.1C9.2,32.8,2.6,22,-13.3,22.3C-29.2,22.7,-54.4,34.3,-69.1,29.8C-83.8,25.2,-88,4.5,-80.2,-9.7C-72.4,-23.8,-52.5,-31.3,-37.1,-36.5C-21.7,-41.7,-10.8,-44.5,-0.6,-43.9C9.7,-43.2,19.5,-39,28.7,-32.7Z" transform="translate(100 100)" />
        </svg> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
  components: {
    
  }
}
</script>

<style scoped>
  .header{
    width: 100vw;
    height: 100vh;
    background: radial-gradient(to bottom, #27282e 0%, #cf7f00 20%);
    background: linear-gradient(180deg, #27282e 0%, #0083cf 40%);
    display: flex;
    flex-direction: row;
  }

  .headerText{
    width: 50vw;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 1rem 3rem;
  }

  .headerImage{
    width: 50vw;
    height: 100%;
    position: relative;
  }
  .headerImage img{
    width: 80%;
    height: auto;
    position: relative;
    filter: drop-shadow(0px 0px 10px rgba(0, 0, 0, .5));
    z-index: 10;
  }

  .info{
    position: absolute;
    background: #454545;
    width: 300px;
    height: 200px;
    top: 370px;
    left: 30px;
    padding: 1rem 2rem;
    border: 3px solid rgba(0, 0, 0, .5);
    box-shadow: 0 0 10px rgba(0, 0, 0, .5);
    z-index: 1;
  }

  .headerText h1{
    text-align:left;
  }

  .headerText h3{
    text-align:left;
    font-size: 1.1rem;
    font-weight: 300;
    line-height: 2rem;
    margin-top: 2rem;
  }
</style>
