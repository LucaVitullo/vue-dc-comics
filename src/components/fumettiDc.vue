<template>
<div class="contents">
     <div class="box" v-for="(card,index) in fumetto" :key="index">
        <img :src="card.thumb" alt="">
        <p>{{card.series}}</p>
    </div>
</div>

</template>
<script>

export default {
    name:'FumettiDc',
    props:["fumetto"]

}
</script>

<style lang="scss" scoped>
.contents{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    color: white;
    column-gap: 3%;
    padding: 30px;
    position: relative;
}
.box{
    width: 200px;
    margin: 15px;
    
}

</style>