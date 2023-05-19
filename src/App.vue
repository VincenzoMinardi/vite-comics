<script>
import PHeader from './components/PHeader.vue'
import PMain from './components/PMain.vue'
import PFooter from './components/PFooter.vue'
import PCard from './components/PCard.vue'

export default{
  components:{
    PHeader,
    PMain,
    PFooter,
    PCard, 
  }
}
</script>

<template>
 <PHeader />
 <PMain />
 <PFooter />
</template>

<style lang="scss">
 @use './assets/styles/partials/variables.scss' as *;
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

 .max-container{
   @include max-container
}
</style>
