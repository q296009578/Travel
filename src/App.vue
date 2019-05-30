<template>
  <div id="app">
    <!-- 这个标签是占位符，表示显示当前路由地址显示的内容 -->
    <keep-alive exclude="Detail">
      <router-view/>
    </keep-alive>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>

</style>
