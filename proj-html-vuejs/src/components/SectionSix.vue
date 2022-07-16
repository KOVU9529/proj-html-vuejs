<template>
<div class="section-six">
    <div class="content-six">
        <div class="six">
            <i class="fa-solid fa-user-group"></i>
            <span >Online Learner</span>
        </div>
         <div class="six"> 
            <i class="fa-solid fa-film"></i>
            <span>Viseo Courses</span>
        </div>
         <div class="six">
            <i class="fa-regular fa-image"></i>
            <span>Sliders & Images</span>
        </div>
         <div class="six">
            <i class="fa-regular fa-thumbs-up"></i>
            <span>Excellent Reviews</span>
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
            padding: 0 10px;
            i{
                font-size: 50px;
                 padding: 0 5px;
            }
        }

    }
}

</style>