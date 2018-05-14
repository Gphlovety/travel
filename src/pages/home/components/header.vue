<template>
  <div class="header">
    <div class="header-left"><div class="iconfont">&#xe624;</div></div>
    <div class="header-input">输入城市/景点/游玩主题</div>
    <div class="header-right">{{this.city}}</div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    line-height: .86rem
    background: $bgColor
    color: #fff
    .header-left
      width: 0.64rem
      float: left;
      text-align: center
      .iconfont
        font-size: .4rem
    .header-input
      flex: 1
      background: #fff
      border-radius: .1rem
      margin: .12rem 0 0 .2rem
      height: .64rem
      line-height: .64rem
      color: #ccc
      padding: 0 0 0 .2rem
      &:before
        font-family: "iconfont"
        content: '\e632'
        margin-right: .08rem
    .header-right
      width: 1.24rem
      text-align: center
      &:after
        font-family: "iconfont"
        content: '\e64a'
        font-size: .24rem
        margin-left: .05rem
</style>
