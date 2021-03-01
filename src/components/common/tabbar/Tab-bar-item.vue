<template>
   <div class="tab-bar-item"  @click="itemclick">
       <div v-if="!isActive"><slot name="item-icon"></slot></div>
       <div v-else><slot name="item-icon-active"></slot></div>
       <div :style = "isStyleActive"><slot name="item-text"></slot></div>
   </div>
</template>

<script>
export default {
    props:{
        path:{
            type:String
        },
        activeStyle: {
                type: String,
                default: 'coral'
            }
    },
   data () {
      return {

      };
   },

   components: {
       
   },

   computed: {
       isActive(){
           return this.$route.path.indexOf(this.path) !== -1
       },
       isStyleActive() {
                return this.isActive ? {color:this.activeStyle} : {}
            }
   },

   methods: {
       itemclick(){
           this.$router.replace(this.path)
       }
   }
}
</script>
<style lang='css' scoped>
.tab-bar-item {
    flex: 1;
    text-align: center;
    height: 49px;
    font-size: 14px;
    color:black;
  }

  .tab-bar-item img {
    width: 24px;
    height: 24px;
    vertical-align: middle;
    margin: 4px 0 2px 0;
  }

</style>