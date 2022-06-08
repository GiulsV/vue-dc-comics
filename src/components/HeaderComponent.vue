<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="DC logo">
      <div id="menu-container">
        <ul>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
          <li><a href="#">games</a></li>
          <li><a href="#">collectibles</a></li>
          <li><a href="#">videos</a></li>
          <li><a href="#">fans</a></li>
          <li><a href="#">news</a></li>
          <li><a href="#">shop</a></li>
        </ul>
      </div>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponent',
}
</script>


<style lang="scss" scoped>

header{
  // background-color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 0rem;
  
  ul{
    display: flex;
    list-style-type: none;
    
    li{
      padding: 0rem 0.8rem;
      font-weight: 600;
      font-size: 16px;
      text-transform: uppercase;
      
      a{
        color: rgb(65, 61, 61);
        text-decoration: none;
      }
    }
  }
}
</style>