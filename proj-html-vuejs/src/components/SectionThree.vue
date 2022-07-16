<template>
  <div class="sectionThree">
      <h2 class="title">NEW COURSES</h2>
    <div class="container">
        <div class="card-img" v-for="card in sectionThreeArray" :key="card.id">
        <div >
         <img :src="card.img" alt="">
         <h2>{{card.title}}</h2>
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
        padding: 40px;
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
        span,
        hr{ color: #aca5b1;}
        hr{
            width: 90%;
            margin:20px auto;
        }
        img{
            width: 100%;
            margin-bottom: 20px;
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
            width: 90%;
            margin: 0 auto;
            i{
                color: #f2ba60;
                margin-right: 5px;
            }
            a{
                color: inherit;
                text-decoration: none;
            }
        }
    }
}
}
</style>

