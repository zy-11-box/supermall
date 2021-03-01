<template>
   <div class="nar-bar">
       <div class="left"><slot name="left"></slot></div>
       <div class="center"><slot name="center">购物街</slot></div>
       <div class="right"><slot name="right"></slot></div>
   </div>
</template>

<script>
export default {
   data () {
      return {

      };
   },

   components: {},

   computed: {},

   methods: {}
}
</script>
<style lang='css' scoped>

.nar-bar {
    display: flex;
    height: 44px;
    line-height: 44px;
    text-align: center;
    box-shadow: 0 1px 1px rgba(100, 100, 100, 0.1);
  }

  .left, .right {
    width: 40px;
  }

  .center {
    flex: 1;
    height: 44px;
  }
</style>