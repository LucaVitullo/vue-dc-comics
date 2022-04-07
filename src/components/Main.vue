<template>
<main>
    <div class="jumbotron">
        <button class="current-series">CURRENT SERIES</button>

    </div>
        <FumettiDc :fumetto='DcComics'/>
        <div class="more">
            <button type="button">LOAD MORE</button>
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
import DcComics from '@/assets/data/DcComics';
import FumettiDc from '@/components/FumettiDc';


export default {
  name: 'MainDiv',
 data(){
     return {DcComics,FumettiDc};
  },
  components:{
      FumettiDc,
    },
};
</script>

<style lang="scss" scoped>
main{
    background-color: black;
}
.more{
    text-align: center;
}
.more button{
    background-color: #0282f9;
    color: white;
    border: 0;
    font-size: 2rem;
    margin-bottom: 10px;
    padding: 10px;
}
.current-series{
    color: white;
    font-size: 2rem;
    background-color: #0282f9;
    position: absolute;
    bottom: -25px;
    left: 100px;
    border: 0;
    padding: 10px;

}
.jumbotron{
        background-image: url(../assets/jumbotron.jpg);
        height: 350px;
        background-size: cover;
        position: relative;
}
.sezione1{
    display: flex;
    color: white;
    justify-content: space-evenly;
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
    column-gap: 50px;
}
.card{
    display: flex;
    align-items: center;
    color: white;
    font-size: 10px;
    padding: 30px;
}
.card img{
    width: 50px;
    margin-right: 10px;
}

</style>