<template>
  <n-space justify="center">
    <n-layout has-sider>
      <n-layout-sider>
        <n-card :bordered="true" class="card" title="Name">
          <template #cover>
            <img
              src="https://07akioni.oss-cn-beijing.aliyuncs.com/07akioni.jpeg"
            />
          </template>
          <template #footer> xxx THB </template>
        </n-card>
      </n-layout-sider>
      <n-layout-sider>
        <n-space vertical class="blist">
          <h2 style="text-align:center">List Order</h2>
          <n-card class="list" title="Name">
            <template #footer>
              <n-space>
                xxx THB
                <n-button class="btn" strong secondary type="primary">-</n-button>
                5
                <n-button class="btn" strong secondary type="primary">+</n-button>
              </n-space>
            </template>
          </n-card>
          <n-card class="list" title="Name">
            <template #footer>
              <n-space>
                xxx THB
                <n-button class="btn" strong secondary type="primary" @click="a">-</n-button>
                5
                <n-button class="btn" strong secondary type="primary" @click="a">+</n-button>
              </n-space>
            </template>
          </n-card>
        </n-space>
        <p>Total xxx THB</p>
          <n-button type="primary" @click="a"> Confirm Order </n-button>
      </n-layout-sider>
    </n-layout>
  </n-space>
</template>

<script>
import { defineComponent } from "vue";
import { NSpace, NCard, NButton, NLayout } from "naive-ui";

export default defineComponent({
  methods: {},
  components: {
    NSpace,
    NCard,
    NButton,
    NLayout,
  },
  setup() {
    // data:[]
    // cart:[]
  },
});
</script>
<style>
.card {
  border-radius: 10mm;
  background-color: rgb(209, 209, 209);
  box-shadow: 1cm;
  width: 200px;
  height: 250px;
  color: green;
  font-weight: bold;
}
.blist{
  background-color: rgb(209, 209, 209);
}
.list {
  background-color: white;
  box-shadow: 1cm;
  width: 250px;
  height: 110px;
  color: green;
  font-weight: bold;
}
.n-button {
  border-radius: 10mm;
  padding: 5mm;
  width: 50mm;
  font-size: 5mm;
}
.btn{
  width: 50px;
  height: 5px;
  background-color: lightgreen;
}
p {
  font-weight: bolder;
  font-size: 30px;
}
</style>
