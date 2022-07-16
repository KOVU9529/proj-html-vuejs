<template>
  <div>
      <nav>
          <div>
              <img src="../assets/images/MasterStudy-1.svg" alt="Logo">
          </div>
          <div class="headerList">
              <ul>
                  <span>NEW</span>
                  <!--Imposto il ciclo v-for
                      Assegno la classe all'elemento attivo-->
                  <li v-for="link,index in links" :key="index">
                      <a @click="active(index)" :href="link.a" :class="{'active' : index === currentActiveElement}">{{link.text}}</a>
                  </li>
              </ul>
              <ul>
                  <li v-for="social,index in socials" :key="index">
                      <a :href="social.a"><i :class="social.class"></i></a>
                  </li>
              </ul>
          </div>
      </nav>
  </div>
</template>

<script>
export default {
    name:'HeaderComponent',
    data(){
        return{
            currentActiveElement:0,
            links:[
                {
                    text:'Courses',
                    a:'#'
                },
                {
                    text:'Course Formats',
                    a:'#'
                },
                {
                    text:'Add Course',
                    a:'#'
                },
                {
                    text:'Pages',
                    a:'#'
                },
                {
                    text:'Demons',
                    a:'#'
                }
            ],
            socials:[
                {
                    class:'fa-brands fa-linkedin',
                    a:'#'
                },
                {
                    class:'fa-brands fa-instagram',
                    a:'#'
                },
                {
                    class:'fa-brands fa-facebook',
                    a:'#'
                },
                {
                    class:'fa-brands fa-twitter',
                    a:'#'
                }
            ]
        }
    },
    methods:{
        active(index){
            this.currentActiveElement=index;
        }
    }
}
</script>

<style lang="scss" scoped>
nav{
    padding: 20px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .headerList{
     display: flex;
      ul{
          position: relative;
          display: flex;
          list-style-type: none;
          span{
              color: white;
              background-color: #dc1246;
              font-size: 10px;
              position: absolute;
              top: -60%;
              left: 62%;
              padding: 2px 4px;
              border-radius: 5px;
          }
             li{
                 padding: 0 10px;
               a{
                text-decoration: none;
                color:#333333 ;
                &:hover{
                    color: #f3c035;
                }
                &.active{
                  border-bottom:3px solid #f3c035;
                }
                } 
            }
        }
    }
}
</style>

