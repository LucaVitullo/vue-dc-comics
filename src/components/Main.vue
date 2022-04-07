<template>
<main>
    <div class="jumbotron"></div>
    <div class="sezione1">
        <div class="contents">
            <fumettiDc :fumetto='item' v-for="(item,index) in fumettiDc" :key="index"/>


        </div>
    </div>
    <div class="sezione2">
        <div class="box-card">
            <div class="card">
                <img src="../assets/buy-comics-digital-comics.png" alt="Digital-comics">
                <p>DIGITAL COMICS</p>
            </div>
            <div class="card">
                <img src="../assets/buy-comics-merchandise.png" alt="Digital-comics">
                <p>DC MERCHANDISE</p>
            </div>
            <div class="card">
                <img src="../assets/buy-comics-subscriptions.png" alt="Digital-comics">
                <p>SUBSCRIPTION</p>
            </div>
            <div class="card">
                <img src="../assets/buy-comics-shop-locator.png" alt="Digital-comics">
                <p>COMIC SHOP LOCATOR</p>
            </div>
            <div class="card">
                <img src="../assets/buy-dc-power-visa.svg" alt="Digital-comics">
                <p>DC POWER</p>
            </div>

        </div>

    </div>
</main>
</template>

<script>
import boxCard from '@/assets/data/dcComics';
import fumettiDc from '@/components/fumettiDc.vue';


export default {
  name: 'MainDiv',
    data(){
    return {boxCard,};
  },
  components:{
      fumettiDc,
    },
};
</script>

<style lang="scss" scoped>
main{
    background-color: black;
}
.jumbotron{
        background-image: url(../assets/jumbotron.jpg);
        height: 350px;
        background-size: cover;
}
.sezione1{
    display: flex;
    height: 500px;
    color: white;
    justify-content: space-evenly;
}
.contents{
    display: flex;
    align-items: center;
    width: 70%;

}

.sezione2{
    background-color: #0282f9;
    display: flex;
    justify-content: space-around;
}
.box-card{
    display: flex;
    width: 70%;
    padding: 30px;
}
.card{
    display: flex;
    align-items: center;
    color: white;
    font-size: 10px;
    padding: 20px;
}
.card img{
    width: 50px;
    margin-right: 10px;
}

</style>