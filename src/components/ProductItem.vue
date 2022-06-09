<template>
    <article>
       <a href="#">
           <img :src="pathImg" :alt="typeProduct">
        </a>
       <a href="#">
           <p> {{title}} </p>
        </a>
    </article> 
</template>

<script>
export default {
     name: 'ProductItem',
     props: {
        product: Object,
        pathImg: String,
        title: String,
        typeProduct: String
    }
}
</script>

<style lang="scss" scoped>
       
</style>