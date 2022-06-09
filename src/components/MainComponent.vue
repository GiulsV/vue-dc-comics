<template>

  <main>
    <div class="jumbotron">
      <div id="label-jumbo">
        <p>current series</p>
      </div>
    </div>
    <div class="container-blue">
      <ProductItem v-for="(item, index) in products" 
        :key="index" 
        :pathImg="item.thumb" 
        :typeProduct="item.type" 
        :title="item.series"
      />
    </div>

   <a id="more-btn" href="#">load more</a>
    
  </main>

</template>

<script>
import ProductItem from '@/components/ProductItem.vue'

export default {
    name: 'MainComponent',
    props: {
      products: Object,
    },
    components: {
      ProductItem
    }
}
</script>

<style lang="scss" scoped>
main{
  background-color: black;
  color: white;
  padding-bottom: 2rem;
  text-align: center;
  .jumbotron{
    background-image: url('@/assets/img/jumbotron.jpg');
    background-position: center top;
    height: 53vh;
    position: relative;

    #label-jumbo{
      position: absolute;
      bottom: -15px;
      left: 125px;
      padding: 0.3rem 2rem;
      background-color: rgb(12, 124, 236);
      color: white;
      text-align: center;
      vertical-align: middle;
      text-transform: uppercase;
      font-size: 24px;
      font-weight: 900;
    }
   
  }
  .container-blue{
        display: flex;
        justify-content: flex-start;
        align-items:flex-start;
        flex-wrap: wrap;
        row-gap: 2rem;
        padding-top: 4rem;
        margin-bottom: 4rem;
  }
   #more-btn{
      background-color: rgb(12, 124, 236);
      padding: 0.7rem 4rem;
      color: white;
      font-size: 12px;
      font-weight: 800;
      text-decoration: none;
      text-transform: uppercase;
        &:hover{
            opacity: 0.8;
            transition: 0.3s;
        }
    }
}
</style>