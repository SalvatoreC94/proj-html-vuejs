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
    message: 'Ciao'
  }
},

components:{
  AppHeader,
  AppMain,
  AppFooter,
},
methods:{
  clicked(){
    alert('Ciao da click')
  }
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

<style scoped>

</style>
