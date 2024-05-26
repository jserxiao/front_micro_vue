<template>
  <div>
    <span class="title" @click="toLogin">子应用vue</span>
  </div>
</template>

<script setup lang="ts">
import { useRouter } from "vue-router";

const { push } = useRouter();
const toLogin = () => {
  push({
    path: "/login",
  });
};
</script>

<style scoped lang="less">
.title {
  color: #fff;
}
</style>
