<template>
  <div class="sectionFour">
      <div class="display">
          <div class="text">
              <h2 class="titleYllow">Get My Exclusive Investing Book just fot $19.50</h2>
              <p>Vestibillum immentum  eu urna vel cursus.
                  Aneam vehicula quam quam, vitae pellentesque urna elementum cursus.
              </p>
              <img src="../assets/images/amazon.png" alt="">
          </div>
          <div class="imgHand">
             <img src="../assets/images/book.png" alt="">
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'SectionFour'
}
</script>

<style lang="scss" scoped>
.sectionFour{
    background-image: url("../assets/images/slider_1-1917x607-1914x606.jpg");
    background-repeat:no-repeat;
    width: 100%;
    .display{
        display: flex;
        align-items: stretch;
        width: 100%;
        .text{
        text-align: center;
        color: white;
        width: 50%;
        padding-top: 15%;
        padding-left:  5%;
        padding-right:  5%;
        .titleYllow{
            color: #f3c035;
        }
    }
    .imgHand{
        display: flex;
        align-items: stretch;
        width: 50%;
        padding-top: 50px;
        img{
            object-fit: contain;
            height: 500px;
            width: 100%; 
            margin-right: 600px;
            &:hover{
                transform: translate(-10px,0px);
                transition: all 2s linear 1s;
            }
        }   
    }
    }
}
</style>

