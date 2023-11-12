<template>
     <n-space vertical>
    <n-space
      vertical
      :style="{
        position: 'fixed',
        top: 0,
        left: 0,
        width: '100%',
        zIndex: 100,
        background: 'white',
        padding: '10px',
      }"
    >
      <n-input-group class="serch">
        <n-icon
          :component="SearchOutline"
          size="35"
          :depth="1"
          style="margin-right: 20px"
        />
        <n-input
          style="
            border-radius: 25px;
            width: 50%;
            justify-content: center;
            height: 35px;
          "
          clearable
          maxlength="50"
          show-count
          placeholder="ค้นหารายชื่อพนักงาน, รหัสพนักงาน"
        >
        </n-input>
      </n-input-group>
    </n-space>
</template>

<script>
import { defineComponent } from '@vue/composition-api'
import {NSpace, NButton } from "naive-ui"

export default defineComponent({
    setup() {
        
    },
})
</script>
<style>

</style>
