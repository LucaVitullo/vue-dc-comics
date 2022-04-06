<template>
<main>
    <div class="sezione1">
        <div class="contents">
            <h1>-->Content goes here >-- </h1>

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
    width: 70vw;
    color: white;
}
.contents{
    display: flex;
    justify-content: space-around;
}

</style>