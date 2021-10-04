<template>
   <section class="banner">
      <div class="container">
          <ul>
              <li><img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">DIGITAL COMICS</li>
              <li><img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">DC MERCHANDISE</li>
              <li><img src="../assets/img/buy-comics-subscriptions.png" alt="sub">SUBSCRIPTION</li>
              <li><img src="../assets/img/buy-comics-shop-locator.png" alt="shop">COMICS SHOP LOCATOR</li>
              <li><img src="../assets/img/buy-dc-power-visa.svg" alt="visa">DC POWER VISA</li>
          </ul>
      </div>
  </section>
</template>

<script>
export default {
    name:"BannerIcons"
}
</script>

<style lang="scss" scope>
@import "../assets/style/common";
@import "../assets/style/variables";
.banner{
    background-color:$defaultColor;
    width:100%;    
    color:white;
    display: flex;    

    ul{
        display: flex;
        justify-content: space-between;
        align-content: center;
        width:100%; 

        li{
        padding:10px 0;
        }

        img{
            height: 45px;
            padding:0 15px;
        }
    }        
}
    
</style>