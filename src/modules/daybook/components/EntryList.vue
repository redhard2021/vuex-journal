<template>
    <div class="entry-list-container">
        <div class="px-2 pt-2">
            <input type="text"
                   class="form-control"
                   placeholder="Search">
        </div>
        <div class="entry-scrollarea">
            <EntryView v-for="item in 100" :key="item"></EntryView>
        </div>
    </div>
</template>

<script>
import { defineAsyncComponent } from '@vue/runtime-core'
export default {
    components:{
        EntryView: defineAsyncComponent(()=> import('./EntryView.vue'))
    }

}
</script>

<style lang="scss" scoped>


.entry-list-container{
    border-right: 1px solid #2c3e50;
    height: calc(100vh - 60px);
}

.entry-scrollarea{
    height: calc(100vh - 115px);
    overflow: scroll;
    overflow-x: hidden;
}
</style>