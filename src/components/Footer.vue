<template>
<footer>
<div class="footer-top">
    <div class="footer-nav">
        <ul>
            <li>
                <h3>DC COMICS</h3>
                <a href="">Characters</a>
                <a href="">Comics</a>
                <a href="">Movies</a>
                <a href="">TV</a>
                <a href="">Games</a>
                <a href="">Videos</a>
                <a href="">News</a>
            </li>
            <li>
                <h3>SHOP</h3>
                <a href="">Shop DC</a>
                <a href="">Shop DC Collectibles</a>
            </li>
        </ul>
        
    </div>
    <div class="footer-nav">

        <ul>
            <li>
                <h3>DC COMICS</h3>
                <a href="">Characters</a>
                <a href="">Comics</a>
                <a href="">Movies</a>
                <a href="">TV</a>
                <a href="">Games</a>
                <a href="">Videos</a>
                <a href="">News</a>
            </li>
        </ul>
        
    </div>
    <div class="footer-nav">
        <ul>
            <li>
                <h3>SITES</h3>
                <a href="">DC</a>
                <a href="">MAD Magazine</a>
                <a href="">DC kids</a>
                <a href="">DC Universe</a>
                <a href="">DC Power Visa</a>
            </li>
        </ul>
        
    </div>
    <div class="contenitore-logo">

    </div>
</div>
<div class="footer-bottom">
    <div class="social">
        <a class="sign-up" href="#">SIGN-UP NOW!</a>
        <div class="social">
          <p>FOLLOW US</p>
          <img src="../assets/footer-facebook.png" alt="facebook" />
          <img src="../assets/footer-twitter.png" alt="facebook" />
          <img src="../assets/footer-youtube.png" alt="facebook" />
          <img src="../assets/footer-pinterest.png" alt="facebook" />
          <img src="../assets/footer-periscope.png" alt="facebook" />
        </div>
    </div>

</div>
</footer>
</template>

<script>
export default {
  name: 'FooterDiv',
}
</script>

<style lang="scss" scoped>

.footer-top{
    background-image:url("../assets/footer-bg.jpg");
    display: flex;
    column-gap: 20px;
    justify-content: flex-end;

}
ul{
    display: flex;
    flex-direction: column;
}
 ul li {
     display: flex;
     flex-direction: column;
     align-items: flex-start;
    color: white;
    padding-bottom: 10px;
     list-style-type: none;

}
.footer-nav{
display: inline-block;
padding-top: 10px;
padding-bottom: 10px;
}
.footer-nav h3{
    color: white;

}

ul li a{
    padding-top: 7px;
    color: gray;
    display: block;
    text-decoration: none;
    &:hover{
        text-decoration: underline;
        color: white;
    }
}
.contenitore-logo{
    background-image:url("../assets/dc-logo-bg.png");
    width: 55%;
    background-repeat: no-repeat;
    background-size: 65% ;
    background-position: center;
    
}

.footer-bottom{
    background-color: #303030;
}

.social{
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 10px;
}

.social .sign-up{
    color: white;
    text-decoration: none;
}
.social *{
    color: blue;
    padding: 5px;
}
.social img{
    padding-left: 15px;
} 
</style>