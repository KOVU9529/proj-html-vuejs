<template>
<div class="section-one">
    <div class="one">
        <h1>START YOUR HUMAN <span>REVOLUTION</span> TODAY</h1>
        <p>A wonderfull serenity has taken possesion of my entire soul, like 
            this sweet mornings of spring which i enjoy with my whole heart.</p>
    </div>
    <div class="back-color">
        <div class="textSection">
            <h2> <span> Limited sale:</span>All courses with 55% off </h2>
         <div  class="immisionOne">
            <input type="text" placeholder="Enter your e-mail">
            <button>SUSCRIBE</button>
         </div>   
        </div>
        <div class="clock">
            <div class="time">{{time}}</div>
            <div >
                <span class="name-clock">Days</span>
                <span class="name-clock">Hours</span>
                <span class="name-clock">Minute</span>
                <span class="name-clock">Second</span>
            </div>

        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'SectionOne',
     //Riporto il valore della props(padre-figlio)
    props:{
        time:Function
    }
}
</script>

<style lang="scss" scoped>
.section-one{
    position: relative;
    background-image: url("../assets/images/slide-1.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    .one{
        width: 25%;
        margin: 0 auto;
        padding:20% 0;
        margin-left: 750px;
        h1{
            font-weight: bold;
            span{
            color: #f3c035;
        }

        }
        
    }    
    .back-color{
        display:flex;
        justify-content: space-between;
        padding: 50px;
        bottom: -10%;
        left: 11%;
        right: 11%;
        position: absolute;
        width: 80%;
        background-color:#f3c035;
        border-radius: 15px;
        .textSection{
            width: 50%;
        }
        .clock{
            text-align: center;
            width: 50%;
            .time{
            font-size: 60px;
            color: white;
        }
        .name-clock{
            padding: 0 15px;
            font-weight: bold;
        }
        }
        
        h2 span{
            color: white;
        }
        .immisionOne{
            position: relative;
            padding-top: 20px ;
            input{
            border: none;
            border-radius: 20px;
            padding: 10px;
            padding-right: 150px;
            outline: none;
            }
            button{
            position: absolute;
            left: 50%;
            border: none;
            border-radius: 20px;
            padding: 10px;
            background-color: #2d4649;
            color: white;
            }
        }
       
    }
}


</style>

