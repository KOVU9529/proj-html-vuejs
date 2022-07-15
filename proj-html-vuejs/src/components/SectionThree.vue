<template>
  <div class="sectionThree">
      <h2 class="title">NEW COURSES</h2>
    <div class="container">
        <div class="card-img" v-for="card in sectionThreeArray" :key="card.id">
        <div >
         <img :src="card.img" alt="">
         <h1>{{card.title}}</h1>
         <span>{{card.sub}}</span>
         <hr>
         <ul>
         <li>
            <i :class="card.iconOne"></i>
            <a :href="card.link">{{card.textOne}}</a>
         </li>
         <li>
            <i :class="card.iconTwo"></i>
            <a :href="card.link">{{card.textTwo}}</a>
         </li>
         <li>
             <i :class="card.iconThree"></i>
            <a :href="card.link">{{card.textThree}}</a>
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
    props:{
        sectionThreeArray:Array
    }
}
</script>

<style lang="scss" scoped>
.sectionThree{
    background-color:#edf2f5 ;
    text-align: center;
    .title{
        padding: 20px;
        font-size: xx-large;
    }
    .container{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    padding: 2% 5%;
    justify-content: space-between;
    .button{
        margin-top: 5% ;
        margin-left: 45%;
        background-color: #f3c035;
        color: white;
        text-decoration: none;
        padding: 15px 20px;
        text-align: center;
        border-radius: 20px;
    }
    .card-img{
        img{
            width: 100%;
        }
        width:calc(96% / 3);
        background-color: white;
        text-align: center;
        margin-top: 10px;
        ul{
            list-style-type: none;
            display: flex;
            justify-content: space-between;
            padding: 5px 10px;
            
            a{
                color: inherit;
                text-decoration: none;
            }
        }
    }
}
}
</style>

