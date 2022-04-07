<template>
    <div class="fumettiDc">
        <img :src="fumetto.thumb" alt="">
        <p>{{fumetto.series}}</p>
    
    </div>
</template>
<script>

export default {
    name:'fumettiDc',
    props:{
        fumetto: Object,

    },

}
</script>

<style lang="scss" scoped>
img{
    height: 100px;
}

</style>