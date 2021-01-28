<template>
  <div id="page" class="">
     <Header/>
      <Menu/>
 
  </div>
  <router-view/>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Menu from '@/components/Menu.vue'



export default {
  name: 'Home',
  components: {
    Header,
    Menu
  }
}
</script>
<style lang="scss">

</style>


