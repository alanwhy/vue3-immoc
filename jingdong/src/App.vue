<template>
  <div>
    <div class="wrapper">
      <div class="position">
        <span class="iconfont position__icon">&#xe619;</span>
        北京理工大学国防科技园2号楼10层
        <span class="iconfont position_notice">&#xe60b;</span>
      </div>
      <div class="search">
        <span class="iconfont">&#xe62d;</span>
        <span class="search__text">山姆会员商店优惠商品</span>
      </div>
      <div class="banner">
        <img
          class="banner__img"
          src="/img/banner.jpg"
        />
      </div>
    </div>
    <div class="docker">
      <div class="docker__item docker__item--active">
        <div class="iconfont">&#xe6f3;</div>
        <div class="docker__title">首页</div>
      </div>
      <div class="docker__item">
        <div class="iconfont">&#xe7e5;</div>
        <div class="docker__title">购物车</div>
      </div>
      <div class="docker__item">
        <div class="iconfont">&#xe61e;</div>
        <div class="docker__title">订单</div>
      </div>
      <div class="docker__item">
        <div class="iconfont">&#xe660;</div>
        <div class="docker__title">我的</div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import "./style/viriables.scss";
@import "./style/mixins.scss";

.wrapper {
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0.5rem;
  right: 0;
  padding: 0 0.18rem;
}
.position {
  position: relative;
  padding: 0.16rem 0.24rem 0.16rem 0;
  line-height: 0.22rem;
  font-size: 0.16rem;
  @include ellipsis;
  .position__icon {
    position: relative;
    top: 0.01rem;
    font-size: 0.2rem;
  }
  .position_notice {
    position: absolute;
    right: 0;
    top: 0.17rem;
    font-size: 0.2rem;
  }
  color: $content-fontcolor;
}

.search {
  margin-bottom: 0.12rem;
  line-height: 0.32rem;
  background: #f5f5f5;
  color: #b7b7b7;
  border-radius: 0.16rem;
  .iconfont {
    display: inline-block;
    padding: 0 0.08rem 0 0.16rem;
    font-size: 0.16rem;
  }
  &__text {
    display: inline-block;
    font-size: 0.14rem;
  }
}

.banner {
  // 防止图片抖动
  height: 0;
  overflow: hidden;
  padding-bottom: 25.4%; // 图片的高宽比
  &__img {
    width: 100%;
  }
}

.docker {
  display: flex;
  box-sizing: border-box;
  position: absolute;
  padding: 0 0.18rem;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 0.49rem;
  border-top: 1px solid #f1f1f1;
  color: $content-fontcolor;
  &__item {
    flex: 1;
    text-align: center;
    .iconfont {
      margin: 0.07rem 0 0.02rem 0;
      font-size: 0.18rem;
    }
    &--active {
      color: #1fa4fc;
    }
  }
  &__title {
    font-size: 20px;
    transform: scale(0.5, 0.5);
    transform-origin: center top;
  }
}
</style>
