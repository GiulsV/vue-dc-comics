<template>
  <div id="app">
    
    <HeaderComponent />

    <main>
      <div>
      <MainComponent/>
      </div>
      <BlueSection/>
    </main>

    <footer>
    <FooterComponent/>
    </footer>
    
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import BlueSection from './components/BlueSection.vue'
import FooterComponent from './components/FooterComponent.vue'

import products from './assets/data/dc-comics'

export default {
  name: 'App',
  data(){
    return{
      products,
    }   
  },

  components: {
    HeaderComponent,
    MainComponent,
    BlueSection,
    FooterComponent,
  }
}
</script>

<style lang="scss">

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
}

.container-footer{
  margin: auto 10%;
}
.container-blue{
  margin: auto 15%;
}
</style>
