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
    padding: 2% 12%;
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
        width:calc(96% / 3);
        background-color: white;
        text-align: center;
        margin-top: 10px;
        h3{
            padding: 5px 20px;
            &:hover{
            color: #f3c035;
        }


        }
        
        span,
        hr{ color: #aca5b1;}
        hr{
            width: 90%;
            margin:20px auto;
        }
        .sectionOverThree{
            position: relative;
            .target{
                border-radius: 5px;
                padding: 4px 2px;
                font-size: 10px;
                position: absolute;
                z-index: 3;
                top: 4px;
                right: 10px;
                color: white;
                background-color: orange ;
            }
            .targetNew{
                border-radius: 5px;
                padding: 4px 2px;
                font-size: 10px;
                position: absolute;
                z-index: 3;
                top: 4px;
                right: 10px;
                color: white;
                background-color: green ;
            }
            .imgOver{
                padding: 25%;
                background-color:rgba($color: #000000, $alpha: 0.5);
                top: 0px;
                position: absolute;
                opacity: 0;
                width: 100%;
                height: 90%;
                .priceOld{
                    text-decoration: line-through;
                    color: #aca5b1;
                }
                .priceNew{
                    color: #f3c035;
                    font-size: 20px;
                }
            }
            img{
            width: 100%;
            height: 220px;
            margin-bottom: 20px;
        } 
        .imgOver:hover{
            opacity: 1;
        }
        }
        ul{
            list-style-type: none;
            display: flex;
            justify-content: space-between;
            padding: 5px 10px;
            width: 90%;
            margin: 0 auto;
            li{
                padding-bottom: 20px ;
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
}
</style>

