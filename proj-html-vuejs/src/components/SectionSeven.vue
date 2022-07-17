<template>
<div class="sevenSelection">
    <h2>What Students Say</h2>
    <div>
        <div class="selection">
            <!--Imposto l'azione indietro al click-->
            <div @click="showPrevElement" class="prev"><i class="fa-solid fa-arrow-left"></i></div>
        <div>
            <!--Imposto l'azione elemento correntemente attivo al click
                più aggiunta classe active-->
            <img @click="sameElement(0)" :class="{'active' : 0 === currentActiveElement}" src="../assets/images/1-100x100.jpg" alt="">
            <img @click="sameElement(1)" :class="{'active' : 1 === currentActiveElement}" src="../assets/images/2-100x100.jpg" alt="">
            <img @click="sameElement(2)" :class="{'active' : 2 === currentActiveElement}" src="../assets/images/4-100x100.jpg" alt="">
        </div>
        <!--Imposto l'azione avanti al click-->
        <div @click="showNextElement" class="next"><i class="fa-solid fa-arrow-right"></i></div>
        </div>
        <div >
            <!--Imposto l'argomentazione per visualizzare l'argomento correntemente attivo-->
            <h3>{{sectionSevenArray[currentActiveElement].title}}</h3>
            <!--Imposto il v-for-->
            <i v-for="star,index in 5" :key="index" class="fa-solid fa-star"></i>
            <div class="paragraph">
                <p>{{sectionSevenArray[currentActiveElement].text}}</p>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'SectionSeven',
    //Riporto il valore della props(padre-figlio)
    props:{
        sectionSevenArray:Array
    },
    data(){
        return{
            //Imposto la variabile partendo da un valore
            currentActiveElement:0,
        }
    },
    methods:{
            //Imposto la funzione per andare indietro
            showPrevElement(){
                //Imposto le condizioni
                if(this.currentActiveElement > 0){
                    this.currentActiveElement--;
                }else{
                    this.currentActiveElement = this.sectionSevenArray.length - 1;
                }
            },
            //Imposto la funzione per andare avanti
            showNextElement(){
                 //Imposto le condizioni
                if(this.currentActiveElement < this.sectionSevenArray.length - 1){
                    this.currentActiveElement++;
                }else{
                    this.currentActiveElement = 0;
                }
            },
            //Imposto la funzione per indicare l'elemento correntemente attivo
            sameElement(elementIndex){
                this.currentActiveElement=elementIndex;
            },
    }
}
</script>
<style lang="scss" scoped>
.sevenSelection{
    padding: 5% 10%;
    text-align: center;
    h2{
        font-size: 40px;
        margin-bottom: 20px;
    }
    .selection{
    padding: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
    .prev,
    .next{
        margin: 0 100px;
        color: black;
        font-weight: 200;
    }
    img{
    width: 100px;
    height: 100px;
    border-radius: 50%;
  margin: 0 10px;
    }
    .active{
        transform: scale(1.2);
    }
}
.fa-solid.fa-star{
    padding: 15px 0;
    color: #f3c035;
}
.paragraph{
    padding: 0 200px;
}
}
</style>
