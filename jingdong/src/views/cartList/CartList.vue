<template>
  <div class="cart">
    <div>作业部分代码，同学尝试实现</div>
    <Docker :currentIndex="1"></Docker>
  </div>
</template>

<script>
import Docker from "./../../components/Docker";
export default {
  name: "CartList",
  components: { Docker },
};
</script>

<style lang="scss" scoped>
.cart {
  margin-top: 0.2rem;
  text-align: center;
}
</style>