<script setup lang="ts">
import { ref } from 'vue'
import request from "./../../utils/request"

defineProps<{ msg: string }>()

const count = ref(0)

request({url: "/lalala", method: "get"}).then((res) => {
  console.log(res);
});
</script>

<template>
  <h1>登陆</h1>
</template>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
