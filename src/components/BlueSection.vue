<template>
  <section>
    <div class="container-blue">
       <div class="container-opzioni">
         <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
         <a href="#">digital comics</a>
       </div>

       <div class="container-opzioni">
         <img src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
         <a href="#">dc merchandise</a>
       </div>

       <div class="container-opzioni">
         <img src="../assets/img/buy-comics-subscriptions.png" alt="digital comics">
         <a href="#">subscription</a>
       </div>

       <div class="container-opzioni">
         <img src="../assets/img/buy-comics-shop-locator.png" alt="digital comics">
         <a href="#">comic shop locator</a>
       </div>

       <div class="container-opzioni">
         <img src="../assets/img/buy-dc-power-visa.svg" alt="digital comics">
         <a href="#">dc power visa</a>
       </div> 
    </div> 
  </section>
</template>

<script>
export default {
    name: 'BlueSection',
}
</script>

<style lang="scss" scoped>
section{
  background-color: rgb(12 124 236);
  
  .container-blue{
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: no-wrap;

        .container-opzioni{
          display: flex;
          align-items: center;
          padding: 4rem 0rem;
          flex-wrap: wrap;
          flex-grow: 1;
          
          img{
            max-height: 60px;
            max-width: 65px;
            margin-right: 0.7rem;
          }

          a{
            color: white;
            text-decoration: none;
            text-transform: uppercase;
            font-size: 14px;
          }
        }
      }
}
</style>