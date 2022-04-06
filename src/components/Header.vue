<template>
<header>
    <div class="header">
    <div class="img">
      <img src="../assets/dc-logo.png" alt="Dc-Logo">
    </div>
    <div class="header-right">
      <ul>
        <li>
          <a href="" v-for="item in navLink" :key="item">
            {{item}}
          </a>
       </li>
     </ul>

    </div>

 
  </div>
</header>

</template>

<script>
export default {
  name: 'HeaderDiv',
  data() {
    return{
    navLink:[
      "CHARACTERS",
      "COMICS",
      "MOVIES",
      "TV",
      "GAMES",
      "COLLECTIBLES",
      "VIDEOS",
      "FANS",
      "NEWS",
      "SHOP",
      ]

    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

 $text-color: black;

.header{
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.header-right ul li{
  list-style-type: none;

}
.header-right li a {
 text-decoration: none;
 margin-left: 15px;
  color: $text-color;
 padding-bottom: 20px;
}
.header-right li a:hover{
  color: blue;
  border-bottom: 2px solid blue;
}


</style>
