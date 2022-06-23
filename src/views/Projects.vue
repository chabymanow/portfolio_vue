<template>
  <div>
    <h1>Let see what we made so far...</h1>
    <div class="projectContent">
        <div class="projectCard" v-for="(product, index) in products"  :key="{ index }">
            <img class="projectImage" :src="product.image" />
            <div class="projectText">
                <p class="projectTitle">{{ product.name}}</p>
                <p class="projectDesc">{{ product.description}}</p>
                <button class="projectButton">See more...</button>
            </div>
            
        </div>
    </div>
  </div>
</template>

<script>
import json from '@/assets/products.json'
export default {
    name: "ProjectPage",
    data(){
        return{
            products: json["products"],
            imagePath: "@/assets/images/products/"
        }
    },
    mounted() {
        this.writeProducts();
    },
    methods:{
        writeProducts(){
            // this.products = json;
            console.log(this.products);
        }
    }

}
</script>

<style scoped>
 h1::before{
    position: absolute;
    content: "Projects";
    font-size: 30rem;
    color: rgba(79, 77, 73, 0.05);
    top: 50px;
    left: -60px;
    z-index: -10;
  }
    .projectContent{
        width: 95vw;
        margin: 0 auto;
        margin-top: 3rem;
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
        gap: 2rem;
        z-index: 1;
        
    }
    .projectCard{
        width: 400px;
        height: 200px;
        position: relative;
        border-radius: 5px;
        overflow: hidden;
        display: flex;
        flex-direction: column;
        background: #FAFAFA;
        box-shadow: 0 0 10px rgba(167, 132, 248, 0.398);
    }

    .projectImage{
        width: 50%;
        height: 100%;        
    }

    .projectText{
        position: absolute;
        top: 0;
        left: 50%;
        right: 0;
        padding: 1rem .5rem;
        color: #2f2f2f;
    }

    .projectTitle{
        font-size: 1.6rem;
        margin-bottom: 1rem;
    }

    .projectDesc{
        font-size: .8rem;
        line-height: 150%;
    }
    .projectButton{
        width: 20ch;
        padding: .3rem 1.5rem;
        margin-top: 2rem;
        background: #ddbc00;
        border: none;
        border-radius: 5px;
    }
</style>