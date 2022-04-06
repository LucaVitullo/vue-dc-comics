<template>
<main>
    <div class="sezione1">
        <div class="contents">
            <h1>-->Content goes here >-- </h1>

        </div>
    </div>
    <div class="sezione2">
        <div class="box-card">
            <div class="card">
                <img src="../assets/buy-comics-digital-comics.png" alt="Digital-comics">
                <span>DIGITAL COMICS</span>
            </div>
            <div class="card">
                <img src="../assets/buy-comics-merchandise.png" alt="Digital-comics">
                <span>DC MERCHANDISE</span>
            </div>
            <div class="card">
                <img src="../assets/buy-comics-subscriptions.png" alt="Digital-comics">
                <span>SUBSCRIPTION</span>
            </div>
            <div class="card">
                <img src="../assets/buy-comics-shop-locator.png" alt="Digital-comics">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div class="card">
                <img src="../assets/buy-dc-power-visa.svg" alt="Digital-comics">
                <span>DC POWER</span>
            </div>

        </div>

    </div>
</main>
</template>

<script>
export default {
  name: 'MainDiv',
  props: {
    msg: String
  }
}
</script>

<style lang="scss" scoped>
main{
    background-color: black;
}
.sezione1{
    display: flex;
    height: 80px;
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
}
.card span{
    margin:20px;
}
</style>