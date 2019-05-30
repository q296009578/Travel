<template>
    <div>
        <detail-banner></detail-banner>
        <detail-header></detail-header>
        <div class="content">
          <detail-list :list="list"></detail-list>
        </div>
    </div>
</template>

<script>
import DetailBanner from './compoments/Banner'
import DetailHeader from './compoments/Header'
import DetailList from './compoments/list'
export default {
  name: 'Detail',
  components: {
    DetailBanner,
    DetailHeader,
    DetailList
  },
  data () {
    return {
      list: [{
        title: '成人票',
        children: [{
          title: '成人三馆联票',
          children: [{
            title: '成人三馆组合票'
          }, {
            title: '成人三馆组合票'
          }]
        }, {
          title: '成人五馆联票'
        }]
      }, {
        title: '儿童票'
      }, {
        title: '特惠票'
      }, {
        title: '学生票'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
    .content
        height 30rem
</style>
