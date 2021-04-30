<template>
  <default-bar />

  <default-view />
  
  <default-directory />

  <default-footer />
</template>

<script>
import { defineAsyncComponent } from 'vue'
  export default {
    name: 'AppLayout',
    components: {
      DefaultBar: defineAsyncComponent(() => import('./AppBar')),
      DefaultView: defineAsyncComponent(() => import('./View')),
      DefaultDirectory: defineAsyncComponent(() => import('./Directory')),
      DefaultFooter: defineAsyncComponent(() => import('./Footer')),
    },
  }
</script>
