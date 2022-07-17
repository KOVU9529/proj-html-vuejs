<template>
<div>
    <div class="containerFooter">
        <div>
          <ul >
            <li>
                <h2>ABOUT</h2>
            </li>
            <li>
               <a class="blu" href="#"> Master Study </a>is education WordPress theme featured by Learning
            </li>
            <li>
                Mangment System (LMS) for online education
            </li>
            <li>
                Developed by <a class="blu" href="#"> StyleixThemes</a>
            </li>
            <li>
                <a href="#"><i class="fa-brands fa-facebook"></i></a> 
                <a href="#"><i class="fa-brands fa-twitter"></i></a> 
                <a href="#"><i class="fa-brands fa-instagram"></i></a> 
            </li>
          </ul>
        </div>
        <div>
            <ul>
                <li>
                    <h2>CONTACT</h2>
                </li>
                <li>
                  USA, Callifornia 20, First Avenue, Callifornia
                </li>
                <li>
                  Tel.: +1 212 458 300 32
                </li>
                <li>
                 Fax: +1 212 375 24 14
                </li>
                <li>
                    <a href="#">info@masterstudy.com</a>
                </li>
            </ul>
        </div>
        <div class="flexUl">
            <ul class="ulPages">
                <li>
                    <h2>
                        PAGES
                    </h2>
                </li>
                <li class="pages">
                   <a  class="overWhite" href="#">Blog</a> 
                </li>
                <li class="pages">
                    <a class="overWhite" href="#">Home</a> 
                </li>
                <li class="pages">
                    <a class="overWhite" href="#">Shortcodes</a> 
                </li>
            </ul>
            <ul >
                <li>
                    <h2 class="comodity">
                        PAGES
                    </h2>
                </li>
                <li class="pages">
                    <a class="overWhite" href="#">Courses</a> 
                </li>
                <li class="pages">
                    <a class="overWhite" href="#">MemberShip A...</a> 
                </li>
                <li class="pages">
                     <a class="overWhite" href="#">Typography</a> 
                </li>
            </ul>
        </div>
        <div class="final">
            <ul>
                <li>
                    <h2>BLOG</h2>
                </li>
                <li class="ulImg">
                    <img src="../assets/images/photo-1517520287167-4bbf64a00d66-50x50.jpeg" alt=""> <div class="partLi"><span class="overWhite"> Our main target is to “Developing Yourself as a Leader” </span>
                    <br><span class="gray"> - August 9, 2018</span></div>
                </li>
                <li class="ulImg">
                    <img src="../assets/images/photo-1490376840453-5f616fbebe5b-50x50.jpeg" alt=""><div class="partLi"><span class="overWhite">Those Other College Expenses You Aren`t Thinking About</span>
                    <br><span class="gray"> - June 3, 2015</span></div>
                </li>
            </ul>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'FooterEnd'
}
</script>

<style lang="scss">
.containerFooter{
    padding: 30px 120px;
    background-color: #f3c035;
    display: flex;
    justify-content: space-between;
    font-size: 12px;
    .blu{
        color: #2d4649;
    }
    .fa-brands.fa-twitter{
        padding: 0 10px;
    }
    ul{
        list-style-type: none;
        li{
            margin-bottom: 10px;
        }
    }
    a{
        text-decoration: none;
        color: inherit;
    }
        .flexUl{
        display: flex;
         .comodity{
            color: #f3c035;
            }
         .ulPages{
            padding-right: 30px;
            }   
        }
    .ulImg{
        display: flex;
        .partLi{
            padding-left: 15px;
        .gray{
            color: #333333;
        }
        }  
    }
    .final{
        margin-left: 10px;
    }
    .overWhite:hover{
        color: white;
    }
    .pages{
        list-style-type: disc;
        &:hover{
        color: white;
    }
    }
}

</style>

