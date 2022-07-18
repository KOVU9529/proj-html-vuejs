<template>
<div class="section-six">
    <div class="content-six">
        <div class="six">
            <i class="fa-solid fa-user-group"></i>
            <div class="sectionNumb">
                <div class="numb">3195</div>
                <span >Online Learner</span>
            </div>
        </div>
         <div class="six"> 
            <i class="fa-solid fa-film"></i>
            <div class="sectionNumb">
                <div class="numb">23</div>
                <span>Video Courses</span>
            </div>
        </div>
         <div class="six">
            <i class="fa-regular fa-image"></i>
            <div class="sectionNumb">
                <div class="numb">437</div>
                <span>Sliders & Images</span>
            </div>
        </div>
         <div class="six">
            <i class="fa-regular fa-thumbs-up"></i>
            <div class="sectionNumb">
                <div class="numb">1440</div>
                <span>Excellent Reviews</span>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'SectionSix'
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