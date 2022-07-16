<template>
  <div id="app">
    <HeaderComponent />
    <SectionOne />
    <SectionTwo />
    <SectionThree :sectionThreeArray="sectionThreeArray"/>
    <SectionFour />
    <SectionFive :sectionFiveArray="sectionFiveArray"/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import SectionOne from './components/SectionOne.vue'
import SectionTwo from './components/SectionTwo.vue'
import SectionThree from './components/SectionThree.vue'
import SectionFour from './components/SectionFour.vue'
import SectionFive from './components/SectionFive.vue'

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
          textOne:'Advanced',
          textTwo:'8 Lectures',
          textThree:'6 Hours'
        },
        {
          id:'2',
          img:require('./assets/images/12345-1-370x200.png'),
          title:'Nvidia and UE4 Technolies Practice',
          sub:'Nvidia',
          textOne:'Advanced',
          textTwo:'8 Lectures',
          textThree:'6 Hours'
        },
        {
          id:'3',
          img:require('./assets/images/photo-1491897554428-130a60dd4757-370x200.jpeg'),
          title:'Fashion Photography from professional',
          sub:'Fashion',
          textOne:'Advanced',
          textTwo:'6 Lectures',
          textThree:'6 Hours'
        },
        {
          id:'4',
          img:require('./assets/images/photo-1416339134316-0e91dc9ded92-370x200.jpeg'),
          title:'Design Instrument for Communications',
          sub:'Communication',
          textOne:'Intermediate',
          textTwo:'6 Lectures',
          textThree:'6 Hours'
        },
        {
          id:'5',
          img:require('./assets/images/cathryn-lavery-67852-unsplash-370x200.jpg'),
          title:'Make your Concept Right and Beautiful',
          sub:'Art',
          link:'#',
          textOne:'Intermediate',
          textTwo:'6 Lectures',
          textThree:'6 Hours'

        },
        {
          id:'6',
          img:require('./assets/images/photo-1475452779376-caebfb988090-370x200.jpeg'),
          title:'Road Bike Manual or how to be a Champion',
          sub:'Bicycling',
          textOne:'Beginner',
          textTwo:'6 Lectures',
          textThree:' 6 Hours'
        }
      ],
      sectionFiveArray:[
        {
          title:'Entrepreneurship',
          icon:'fa-solid fa-briefcase',
          text:'Vestibulum vitae aliquam nunc.Suspendisse mollis metus ac tellus egestus pharetra.Suspendisse at viverra purus.Pellentesque nec posuere ligula,eu congue leo.Integer vulputate tempor arcu.Vestibulum vulputate'
        },
        {
          title:'Accellerated learning',
          icon:'fa-solid fa-rocket',
          text:'Vestibulum vitae aliquam nunc.Suspendisse mollis metus ac tellus egestus pharetra.Suspendisse at viverra purus.Pellentesque nec posuere ligula,eu congue leo.Integer vulputate tempor arcu.Vestibulum vulputate'
        },
        {
          title:'Productivity',
          icon:'fa-regular fa-thumbs-up',
          text:'Vestibulum vitae aliquam nunc.Suspendisse mollis metus ac tellus egestus pharetra.Suspendisse at viverra purus.Pellentesque nec posuere ligula,eu congue leo.Integer vulputate tempor arcu.Vestibulum vulputate'
        },
        {
          title:'Life Coaching',
          icon:'fa-solid fa-gear',
          text:'Vestibulum vitae aliquam nunc.Suspendisse mollis metus ac tellus egestus pharetra.Suspendisse at viverra purus.Pellentesque nec posuere ligula,eu congue leo.Integer vulputate tempor arcu.Vestibulum vulputate'
        }
        

      ]
    }
  },
  components: {
    HeaderComponent,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive
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
