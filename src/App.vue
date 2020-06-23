<template>
  <div ref="root"></div>
</template>

<script lang="ts">
import { defineComponent, onMounted, ref } from 'vue'

export default defineComponent({
    name: 'App',
    setup() {
        const root = ref(null)
        onMounted(() => {
            console.log(root.value)
        })
    }
})
</script>
<style lang="stylus">
  #app {
    img {
      width: 100px;
    }
  }
</style>
