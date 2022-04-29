<script lang="ts">
import { defineComponent } from 'vue'
import { Teleport, Suspense } from 'vue'

export default defineComponent({
  components: { Teleport, Suspense},
})
</script>

<template>
  <component :is="Math.random() > 0.5 ? 'Teleport' : 'Suspense'" :to="body">
    This is the real content  
  </component> 
</template>

