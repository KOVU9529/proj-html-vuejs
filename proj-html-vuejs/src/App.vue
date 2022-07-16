<template>
  <div id="app">
    <HeaderComponent />
    <SectionOne :time="time"/>
    <SectionTwo />
    <SectionThree :sectionThreeArray="sectionThreeArray"/>
    <SectionFour />
    <SectionFive :sectionFiveArray="sectionFiveArray"/>
    <SectionSix />
    <SectionSeven :sectionSevenArray="sectionSevenArray"/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import SectionOne from './components/SectionOne.vue'
import SectionTwo from './components/SectionTwo.vue'
import SectionThree from './components/SectionThree.vue'
import SectionFour from './components/SectionFour.vue'
import SectionFive from './components/SectionFive.vue'
import SectionSix from './components/SectionSix.vue'
import SectionSeven from './components/SectionSeven.vue'

import dayjs from 'dayjs'


export default {
  name: 'App',
  data(){
    return{
      time:dayjs().format('DD HH mm ss'),
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
        

      ],
      sectionSevenArray:[
        {
          title:'Come as you are',
          text:'MasterStudy used is an excellent workshop whether you come as a counselor, advisor, administrator, or faculty member. I am going home empowered. I am looking forward to attending the On Course MasterStudy and the MasterStudy National Conference next year and facilitating the use of this excellent retention/student success course at my college.Paints of the FutureThe response to your MasterStudy has been really overwhelming! Those who participated in the workshop are spreading the word here on campus and the “buzz” is on. The VP of Instruction wants you to come back! Her goal is to have more faculty trained. She also w'
        },
        {
          title:'Paints of the Future',
          text:'The response to your MasterStudy has been really overwhelming! Those who participated in the workshop are spreading the word here on campus and the “buzz” is on. The VP of Instruction wants you to come back! Her goal is to have more faculty trained. She also wants to attend a workshop herself. Our President told me Masterstudy needs to be the cornerstone of our success program.”Investing for Your FutureIt is no exaggeration to say this MasterStudy experience was transformative–both professionally and personally. This workshop will long remain a high point of my life. Thanks again…. I am feeling energized and eager to start teaching my class next week. I can’t wait to use all of my new teaching tools. I will absolutely recommend this workshop to other educators!'
        },
        {
          title:'Investing of Your Future',
          text:'It is no exaggeration to say this MasterStudy experience was transformative-both professionally and personally.This workshop will long remain a high point of my life. Thanks again…. I am feeling energized and eager to start teaching my class next week. I can’t wait to use all of my new teaching tools. I will absolutely recommend this workshop to other educators!'
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
    SectionFive,
    SectionSix,
    SectionSeven
  }
}
</script>

<style lang="scss">
*{
  margin: 0%;
  padding: 0%;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
</style>
