<template>
  <footer>
    <div class="container-footer">
      <div class="container-list">
        <ul>
          <li>dc comics</li>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>

        <ul>
          <li>shop</li>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </div>

      <div class="container-list">
        <ul>
          <li>dc</li>
          <li>Terms Of Use</li>
          <li>Privacy policy (News)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>
      </div>

      <div class="container-list">
        <ul>
          <li>sites</li>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div> 
    </div>

    <div class="social-container">
      <a class="btn" href="#nowhere">sign-up now!</a>
      <div class="icons">
        <span>follow us</span>
        <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook icon"></a>
        <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter icon"></a>
        <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube icon"></a>
        <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest icon"></a>
        <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope icon"></a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterComponent',
}
</script>

<style lang="scss" scoped>

footer{
    background-image: url('../assets/img/dc-logo-bg.png'), url('../assets/img/footer-bg.jpg');
    background-position: right bottom, left top;
    background-size: 500px 450px, 100% 100%;
    background-repeat: no-repeat;
    background-origin: content-box;
    overflow-x: hidden;
  .container-footer{
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    .container-list{
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      margin-right: 4rem;
      padding-top: 1.5rem;

      ul{
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: flex-start;
        margin-bottom: 0.8rem;
        list-style-type: none;

        li{
          color: grey;
          padding: 0.3rem;
          font-size: 14px;
          a{
            text-decoration: none;
            color: grey;
          }
          &:first-of-type{
            font-size: 18px;
            font-weight: 700;
            text-transform: uppercase;
            color: white;
      }
    }
    }
  }
}
.social-container{
      
      background-color: rgb(48 48 48);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 100px;  
      column-gap: 1rem;
     a.btn{
        color: white;
        font-size: 16px;
        padding: 1rem 2rem;
        border: 2px solid rgb(12 124 236);
        text-decoration: none;
        text-transform: uppercase;
      }
      span{
        text-transform: uppercase;
        font-size: 16px;
        font-weight: 700;
        color: rgb(12 124 236);
        vertical-align: middle;
        
      }
     .icons{
       display: flex;
       justify-content: flex-start;
       align-items: center;
       flex-wrap: wrap;
       row-gap: 0.5rem;
       column-gap: 0.5rem;
         
        img{
        vertical-align: middle;
        color: rgb(12 124 236);
        padding: 0rem 0.5rem;
        } 
     } 
    }   
  }
</style>