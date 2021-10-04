<template>
     <footer>
          <section class="footer-top">
               <div class="container">
                    <div class="lista">
                         <h3>DC COMICS</h3>
                         <ul>
                              <li>link</li>
                              <li>link</li>
                         </ul>
                         <h3>SHOP</h3>
                         <ul>
                              <li>link</li>
                              <li>link</li>
                         </ul>
                    </div>
                    <div class="lista">
                         <h3>DC </h3>
                         <ul>
                              <li>link</li>
                              <li>link</li>
                              <li>link</li>
                              <li>link</li>
                              <li>link</li>
                              <li>link</li>
                         </ul>
                    </div>
                    
               </div>
          </section>
          <section class="footer-bottom">
               <div class="container">
                    <button>SIGN-UP NOW</button>
                    <div class="social">
                         <img src="../assets/img/footer-facebook.png" alt="fb">
                         <img src="../assets/img/footer-periscope.png" alt="periscope">
                         <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                         <img src="../assets/img/footer-twitter.png" alt="twitter">
                         <img src="../assets/img/footer-youtube.png" alt="yt">
                    </div>
               </div>
          </section>
     </footer>
</template>

<script>
export default {
     name:"Footer"
}
</script>

<style lang="scss" scope>
.footer-top{
     background-image: url('../assets/img/footer-bg.jpg');
     width:100%;
     display: flex;
     color: white;
     padding:50px 0;
     
.container{
     display: flex;
     width:50%;
     justify-content: flex-start;
}
     .lista{
     margin: 0 50px;
     
          ul{
          list-style: none;
          display:flex;
          }
     }
     
}
.footer-bottom{
     background-color: #303030;
     display: flex;
     justify-content: space-between;

     button{
          margin: 20px;
          background-color:#303030 ;
          border: 2px solid #0282f9;
          padding: 5px 10px;
          color: white;

     }
     img{
          
          padding:15px;
     }
}
</style>