<template>
  <div class="sectionFive">
      <h2>Why my Courses?</h2>
      <div class="containerFive">
          <div class="cardCourses" v-for="card,index in sectionFiveArray" :key="index">
            <div>
                 <i :class="card.icon"></i> 
            </div>
           
            <div>
                <h3> {{card.title}}</h3>
            <p>
                {{card.text}}
            </p>
            </div>
            
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'SectionFive',
    props:{
        sectionFiveArray:Array
    }
}
</script>

<style lang="scss" scoped>
.sectionFive{
     width: 100%;
     text-align: center;
     padding: 10px;
     h2{
        font-size: 40px;
        padding: 20px;
     }
    .containerFive{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    width: 60%;
    margin: 0 auto;
    text-align: left;
    .cardCourses{
        display: flex;
        width: 48%;
        border-left: 3px solid #f3c035;
        padding: 20px 10px;
        margin-bottom: 15px;
        box-shadow:5px 5px rgba($color: #9c9693, $alpha: 0.1);
        &:hover {
            background-color: #f3c035;
        }
         &:hover i{
             color: white;
         }
        i{
            color: #f3c035;
            font-size: 50px;
            padding: 0 20px;
            }
        h3{
            padding-bottom: 10px;
        }
        p{
            color: #9c9693;
        }
    }
}

}


</style>

