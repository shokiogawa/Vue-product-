<template>
  <div id="app">
   <product-list v-bind:products="products"></product-list>
  </div>
</template>

<script>
import productList from './components/product-list.vue'

export default {
  name: 'App',
  components: {
    'product-list' : productList
  },
  data: function(){
    return {
      products: [
        {id: 1,name: 'Michael<br>スマホケース', price: 1580, image: require('./assets/images/9125.jpg'), delv: 0, isSale: true},
        {id: 2,name: 'Raphel<br>スマホケース',price: 1580, image: require('./assets/images/9131.jpg'), delv: 0, isSale: true},
        {id: 3,name: 'Gabriel<br>スマホケース',price: 1580, image: require('./assets/images/9800.jpg'), delv: 240, isSale: true},
        {id: 4,name: 'Uriel<br>スマホケース',price: 980, image: require('./assets/images/9909.jpg'), delv: 0, isSale:true},
        {id: 5,name: 'Ariel<br>スマホケース', price: 980, image: require('./assets/images/9913.jpg'), delv: 0, isSale:false},
        {id: 6,name: 'Azrael<br>スマホケース',price: 1580, image: require('./assets/images/10648.jpg'), delv: 0,isSale:false},
      ]
    }
  }
}
</script>

<style>
body{
  background :#000;
  color:#fff;
}
</style>
