<script setup>
import { ref } from "vue";
const show = ref(false);
</script>

<template>
  <button @click="show = !show">toggleShow</button>
  <div>
    show:<span>{{ show }}</span>
  </div>
  <van-dialog v-model:show="show" title="标题" show-cancel-button>
    <img src="https://fastly.jsdelivr.net/npm/@vant/assets/apple-3.jpeg" />
  </van-dialog>
</template>
