<template>
  <div id="app">
    <HeaderComponent />
    <SectionOne />
    <SectionTwo />
    <SectionThree :sectionThreeArray="sectionThreeArray"/>
    <SectionFour />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import SectionOne from './components/SectionOne.vue'
import SectionTwo from './components/SectionTwo.vue'
import SectionThree from './components/SectionThree.vue'
import SectionFour from './components/SectionFour.vue'


export default {
  name: 'App',
  data(){
    return{
      sectionThreeArray:[
        {
          id:'1',
          img:require('./assets/images/photo-1496307042754-b4aa456c4a2d-370x200.jpeg'),
          title:'How to be a dj? Make Eletronic Music',
          sub:'Eletronic',
          iconOne:'fa-solid fa-signal-bars-good',
          icontwo:'fa-brands fa-facebook',
          iconthree:'fa-solid fa-clock-five',
          link:'#',
          textOne:'Advanced',
          textTwo:'Lectures',
          textThree:'Hours'
        },
        {
          id:'2',
          img:require('./assets/images/12345-1-370x200.png'),
          title:'Nvidia and UE4 Technolies Practice',
          sub:'Nvidia',
          iconOne:'fa-solid fa-signal-bars-good',
          icontwo:'',
          iconthree:'fa-regular fa-clock-five',
          link:'#',
          textOne:'Advanced',
          textTwo:'Lectures',
          textThree:'Hours'
        },
        {
          id:'3',
          img:require('./assets/images/photo-1491897554428-130a60dd4757-370x200.jpeg'),
          title:'Fashion Photography from professional',
          sub:'Fashion',
          iconOne:'fa-solid fa-signal-bars-good',
          icontwo:'',
          iconthree:'fa-regular fa-clock-five',
          link:'#',
          textOne:'Advanced',
          textTwo:'Lectures',
          textThree:'Hours'
        },
        {
          id:'4',
          img:require('./assets/images/photo-1416339134316-0e91dc9ded92-370x200.jpeg'),
          title:'Design Instrument for Communications',
          sub:'Communication',
          iconOne:'fa-solid fa-signal-bars-good',
          icontwo:'',
          iconthree:'fa-regular fa-clock-five',
          link:'#',
          textOne:'Intermediate',
          textTwo:'Lectures',
          textThree:'Hours'
        },
        {
          id:'5',
          img:require('./assets/images/cathryn-lavery-67852-unsplash-370x200.jpg'),
          title:'Make your Concept Right and Beautiful',
          sub:'Art',
          iconOne:'fa-solid fa-signal-bars-good',
          icontwo:'',
          iconthree:'fa-regular fa-clock-five',
          link:'#',
          textOne:'Intermediate',
          textTwo:'Lectures',
          textThree:'Hours'

        },
        {
          id:'6',
          img:require('./assets/images/photo-1475452779376-caebfb988090-370x200.jpeg'),
          title:'Road Bike Manual or how to be a Champion',
          sub:'Bicycling',
          iconOne:'fa-solid fa-signal-bars-good',
          icontwo:'',
          iconthree:'fa-regular fa-clock-five',
          link:'#',
          textOne:'Beginner',
          textTwo:'Lectures',
          textThree:'Hours'
        }
      ]
    }
  },
  components: {
    HeaderComponent,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour
  }
}
</script>

<style lang="scss">
*{
  margin: 0%;
  padding: 0%;
  box-sizing: border-box;
}
</style>
