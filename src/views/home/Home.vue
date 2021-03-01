<template>
   <div id="home">
      <nav-bar class="home-nav">
         <div id="center"></div>
      </nav-bar>
   </div>
</template>

<script>
import NavBar from 'components/common/nav/NavBar.vue';
export default {
   data () {
      return {

      };
   },

   components: {
      NavBar
      },

   computed: {},

   methods: {}
}
</script>
<style lang='css' scoped>
.home-nav{
   background-color: pink;
   color: #f0f0f0;
   font-size: 20px;
}
</style>
