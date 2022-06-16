<script setup>
import { ref } from "vue";
const show = ref(false);
</script>
<script>
import { Dialog } from "vant";

export default {
  components: {
    [Dialog.Component.name]: Dialog.Component,
  },
};
</script>

<template>
<button @click="show=!show">toggle</button>
  <van-dialog v-model:show="show" title="标题" show-cancel-button>
    <img src="https://fastly.jsdelivr.net/npm/@vant/assets/apple-3.jpeg" />
  </van-dialog>
</template>
