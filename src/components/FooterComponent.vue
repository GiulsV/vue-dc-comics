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
  </footer>
</template>

<script>
export default {
    name: 'FooterComponent',
}
</script>

<style lang="scss" scoped>

footer{
  background-image: url('../assets/img/footer-bg.jpg');
  background-position: top;
  background-size: 100%;
  background-repeat: no-repeat;
  display: flex;
  height: 50vh;
  .container-footer{
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    .container-list{
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      margin-right: 4rem;

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
}
</style>