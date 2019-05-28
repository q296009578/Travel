<template>
    <div>
        <div class="title">周末去哪儿</div>
        <ul>
            <li v-for="item of recommendList" :key="item.id" class="item border-bottom">
                <div class="item-img-wraper">
                    <img :src="item.imgUrl" alt="" class="item-img">
                </div>
                <div class="item-info">
                    <p class="item-title">{{item.title}}</p>
                    <p class="item-desc">{{item.desc}}</p>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1811/b8/5d599bbdcf8b57.jpg_r_640x214_2ee055e3.jpg',
        title: '大连的海洋世界',
        desc: '大连的海洋世界'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1811/b8/5d599bbdcf8b57.jpg_r_640x214_2ee055e3.jpg',
        title: '大连的海洋世界',
        desc: '大连的海洋世界'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
@import '~styles/mixins.styl'
    .title
        margin-top .2rem
        line-height .8rem
        background #eee
        text-indent .2rem
    .item-img-wraper
        overflow hidden
        height 0
        padding-bottom 33.9%
        .item-img
            width 100%
    .item-info
        padding .1rem
        .item-title
            line-height .54rem
            font-size .32rem
            ellipsis()
        .item-desc
            line-height .4rem
            color #ccc
            ellipsis()
</style>
