<template>
  <div class="dislpayCard">
    <div class="cardText">
      <h2>
        Hei there my name is Jon Doe. I'm the founder of the Brayn Accademy.
      </h2>
      <img src="../assets/images/firma.png" alt="">
    </div>
    <div class="cardText">
      <p>
        A wonderful serenity has taken possession of my entire soul, 
        like these sweet mornings of spring which I enjoy with my whole heart. 
        I am alone, and feel the charm of existence in this spot, 
        which was created for the bliss of souls like mine. 
        I am so happy, my dear friend, so absorbed in the exquisite sense of mere tranquil existence, 
        that I neglect my talents. 
        I should be incapable of drawing a single stroke at the present moment; 
        and yet I feel that I never was a greater artist than now. 
        When, while the lovely valley teems with vapour around me, 
        and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, 
        and but a few stray gleams steal into the inner sanctuary
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name:'SectionTwo'
}
</script>

<style lang="scss" scoped>
.dislpayCard{
  display: flex;
  width: 100%;
  padding: 5% 20%;
  .cardText{
    width: 50%;
    padding: 20px 60px;
  }
}
</style>

