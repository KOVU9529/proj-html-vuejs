<template>
  <div class="sectionThree">
      <h2 class="title">NEW COURSES</h2>
    <div class="container">
        <!--Imposto il ciclo v-for per stampare le card-->
        <div class="card-img" v-for="card in sectionThreeArray" :key="card.id">
        <div >
            <div class="sectionOverThree">
                 <img :src="card.img" alt="">
                 <!--Assegno determinate classi se e solo se sono soddisfatti determinati valori-->
                 <span v-if="(card.target === 'NEW')" :class="{'targetNew':card.target === 'NEW' }" >{{card.target}}</span>
                 <span v-else :class="{'target':card.target === 'SPECIAL' }" >{{card.target}}</span>
                 <div class="imgOver"><span class="priceOld">{{card.priceOld}}</span > <span class="priceNew">{{card.priceNew}}</span> </div>
            </div>
         <h3>{{card.title}}</h3>
         <span>{{card.sub}}</span>
         <hr>
         <ul>
         <li>
           <i class="fa-solid fa-signal"></i>
            <a href="#">{{card.textOne}}</a>
         </li>
         <li>
            <i class="fa-solid fa-bars"></i>
            <a href="#">{{card.textTwo}}</a>
         </li>
         <li>
            <i class="fa-regular fa-clock"></i>
            <a href="#">{{card.textThree}}</a>
         </li>
         </ul>
        </div>
    </div>
    <a class="button" href="#">LOAD MORE</a>
    </div>
  </div>
</template>

<script>
export default {
    name:'SectionThree',
    //Riporto il valore della props(padre-figlio)
    props:{
        sectionThreeArray:Array
    }
}
</script>

<style lang="scss" scoped>
//importo il css
@import  '@/assets/scss/styleThree.scss';
</style>

