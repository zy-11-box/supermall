<template>
   <div id="app">
      <tab-bar>
         <tab-bar-item path="/home" >
            <img  slot="item-icon" src="~assets/img/tabbar/home.svg" alt="">
            <img  slot="item-icon-active" src="~assets/img/tabbar/home_active.svg" alt="">
            <div slot="item-text">首页</div>
         </tab-bar-item>
         <tab-bar-item path="/category" >
            <img  slot="item-icon" src="~assets/img/tabbar/category.svg" alt="">
            <img  slot="item-icon-active" src="~assets/img/tabbar/category_active.svg" alt="">
            <div slot="item-text">品类</div>
         </tab-bar-item>
         <tab-bar-item path="/cart" >
            <img  slot="item-icon" src="~assets/img/tabbar/shopcart.svg" alt="">
            <img  slot="item-icon-active" src="~assets/img/tabbar/shopcart_active.svg" alt="">
            <div slot="item-text">购物车</div>
         </tab-bar-item>
         <tab-bar-item path="/me" >
            <img  slot="item-icon" src="~assets/img/tabbar/profile.svg" alt="">
            <img  slot="item-icon-active" src="~assets/img/tabbar/profile_active.svg" alt="">
            <div slot="item-text">我的</div>
         </tab-bar-item>
      </tab-bar>
      <router-view></router-view>
   </div>
</template>

<script>
import TabBarItem from 'components/common/tabbar/Tab-bar-item.vue';
import TabBar from 'components/common/tabbar/Tab-bar.vue';
export default {
   data () {
      return {

      };
   },

   components: {
      TabBar,
      TabBarItem,
   },

   computed: {},

   methods: {}
}
</script>
<style lang='css' scoped>
@import "assets/css/base.css";
</style>
