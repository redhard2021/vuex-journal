<template>
  <div class="d-flex justify-content-center">
    <h1 class="align-self-center">No select</h1>
    <FaBtn/>
  </div>
</template>

<script>
import { defineAsyncComponent } from '@vue/runtime-core'
export default {
    components:{
        FaBtn: defineAsyncComponent(()=> import('@/modules/daybook/components/FaBtn.vue'))
    }
}
</script>

<style lang="scss" scoped>
div{
    height: 100%;
}
</style>