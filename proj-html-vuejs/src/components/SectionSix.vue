<template>
<div class="section-six">
    <div class="content-six">
        <div class="six">
            <i class="fa-solid fa-user-group"></i>
            <div class="sectionNumb">
                <div class="numb">{{onlineLearner}}</div>
                <span >Online Learner</span>
            </div>
        </div>
         <div class="six"> 
            <i class="fa-solid fa-film"></i>
            <div class="sectionNumb">
                <div class="numb">{{videoCourses}}</div>
                <span>Video Courses</span>
            </div>
        </div>
         <div class="six">
            <i class="fa-regular fa-image"></i>
            <div class="sectionNumb">
                <div class="numb">{{slidersImages}}</div>
                <span>Sliders & Images</span>
            </div>
        </div>
         <div class="six">
            <i class="fa-regular fa-thumbs-up"></i>
            <div class="sectionNumb">
                <div  class="numb">{{excellentReviews}}</div>
                <span>Excellent Reviews</span>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'SectionSix',
    data(){
        return{
            //creo le variabili flag
             onlineLearner: 1,
             videoCourses:1,
             slidersImages:1,
             excellentReviews:1,
             autoPlusNumb:null,
        }
    },
    methods:{ 
        //imposto le funzioni che aumentano i valore numerico
        plusNumbOne(){
            if(this.onlineLearner < 3195){
                this.onlineLearner ++
            }
        },
        plusNumbTwo(){
            if(this.videoCourses < 23){
                this.videoCourses ++
            }
        },
        plusNumbThree(){
            if(this.slidersImages < 437){
                this.slidersImages ++
            }
        },
         plusNumbFour(){
            if(this.excellentReviews < 1440){
                this.excellentReviews ++
            }
        }
    },
    mounted(){
        //imposto il tempo d'azione delle funzioni
        this.autoPlusNumb=setInterval(this.plusNumbOne,10);
        this.autoPlusNumb=setInterval(this.plusNumbTwo,10);
        this.autoPlusNumb=setInterval(this.plusNumbThree,10);
        this.autoPlusNumb=setInterval(this.plusNumbFour,10); 
    }
}
</script>

<style lang="scss" scoped>
.section-six{
    background-image: url("../assets/images/counter-1919x1101.jpg");
    width: 100%;
    .content-six{
        display: flex;
        justify-content: center;
        padding: 250px;
        color: white;
        .six{
            display: flex;
            padding: 0 10px;
            .sectionNumb{
                padding-left:10px;
                .numb{
                font-weight: bold;
                font-size: 30px;
                color: #f3c035;
            }
            }
            i{
                font-size: 50px;
                padding: 0 5px;
            }
        }
    }
}
</style>