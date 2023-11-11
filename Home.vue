<template>
  <n-space justify="center">
    <h1>Billionaire Store</h1>
  </n-space>
  <n-space justify="center">
    <n-button class="button" type="primary" v-show="isManager = true">Manage Employee</n-button>
    <n-button class="button" type="primary" v-show="isEmployee = true">Point of Sell</n-button>
    <n-button class="button" type="primary" v-show="isEmployee = true">Manage Product Inventory</n-button>
    <n-button class="button" type="primary" v-show="isEmployee = true">Manage Product Shelf</n-button>
  </n-space>
</template>

<script>
import {NSpace, NButton } from "naive-ui";


export default {
  name: "App",

  components: {
    NSpace,
    NButton,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1 {
  text-align: center;
  justify-content: center;
  font-size: 20mm;
  font-weight: 800;
}
.button{
  font-size: 1vw;
  width: 300px;
  height:150px;
}
</style>
