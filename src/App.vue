<template>
  <div id='app'>
    <router-view></router-view>
    <tab-bar>
      <tab-bar-item  path = "/home">
        <img slot="itemimg" src="@/assets/img/tabbar/shouye.png" alt="">
        <img slot="itemimga" src="@/assets/img/tabbar/shouye-a.png" alt="">
        <div slot="itemtext">首页 </div>
      </tab-bar-item>
       <tab-bar-item path="/category">
        <img slot="itemimg" src="@/assets/img/tabbar/fenlei.png" alt="">
        <img slot="itemimga" src="@/assets/img/tabbar/fenlei-a.png" alt="">
        <div slot="itemtext">分类 </div>
      </tab-bar-item>
      <tab-bar-item path="/cart">
        <img slot="itemimg" src="@/assets/img/tabbar/gouwuche.png" alt="">
        <img slot="itemimga" src="@/assets/img/tabbar/gouwuche-a.png" alt="">
        <div slot="itemtext">购物车 </div>
      </tab-bar-item>
       <tab-bar-item path="/profile">
        <img slot="itemimg" src="@/assets/img/tabbar/wode.png" alt="">
        <img slot="itemimga" src="@/assets/img/tabbar/wode-a.png" alt="">
        <div slot="itemtext">我的 </div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
const TabBar = ()=> import('components/common/tabbar.vue')
const TabBarItem = ()=> import('components/common/tabbaritem.vue')
export default {

  components: {
    TabBar,
    TabBarItem
  }

}
</script>

<style>

</style>