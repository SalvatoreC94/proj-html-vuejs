<script>

// 1 Importazione del componente
// 2 Dichiarazione del componente
// 3 Utilizzo del componente

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default{
data(){
  return{
   
  }
},

components:{
  AppHeader,
  AppMain,
  AppFooter,
},
methods:{
  
}
}
</script>

<template>
  <div>
   <AppHeader/>
   <AppMain/>
   <AppFooter/>
  </div>
</template>

<style lang="scss">

</style>
