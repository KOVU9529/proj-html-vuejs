<template>
  <div class="sectionFour">
      <div class="display">
          <div class="text">
              <h2 class="titleYllow">Get My Exclusive Investing Book just fot $19.50</h2>
              <p>Vestibillum immentum  eu urna vel cursus.
                  Aneam vehicula quam quam, vitae pellentesque urna elementum cursus.
              </p>
              <a href="#"><img src="../assets/images/amazon.png" alt=""></a>
          </div>
          <div class="imgHand">
            <img src="../assets/images/book.png" alt="">
          </div>
          <div>
              <nav class="navBar">
                  <a href="#"><i class="fa-solid fa-desktop"></i></a>
                  <a href="#"><i class="fa-solid fa-gear"></i></a>
                  <a href="#"><i class="fa-solid fa-wrench"></i></a>
                  <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
                  <a href="#"><i class="fa-solid fa-mobile-screen-button"></i></a>
              </nav>
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
    overflow: hidden;
    background-image: url("../assets/images/slider_1-1917x607-1914x606.jpg");
    background-repeat:no-repeat;
    width: 100%;
    
    .display{
        display: flex;
        align-items: stretch;
        width: 100%;
          &:hover > .imgHand{
                transform: translate( -20px , 10px);
                transition: all 2s linear 1s;
            }
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
            transform: scale(1.1);
           
        }   
    }
    .navBar{
        margin-top: 30px;
        padding: 15px;
        background-color: white;
        display: flex;
        flex-direction: column;
        i{
            color: #5c544d;
            padding: 10px 0;
        }
    }
    }
}
</style>

