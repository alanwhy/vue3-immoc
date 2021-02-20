<template>
  <div class="mine">
    <div>开发中...</div>
    <Docker :currentIndex="3"></Docker>
  </div>
</template>

<script>
import Docker from "./../../components/Docker";
export default {
  name: "Mine",
  components: { Docker },
};
</script>

<style lang="scss" scoped>
.mine {
  margin-top: 0.2rem;
  text-align: center;
}
</style>