<template>
  <div class="kkl-footer">
    <div class="container">
      <links />
    </div>
  </div>
</template>

<script>
  // Components
  import Links from '@/common/components/Links'
  export default {
    name: 'DefaultFooter',
    components: { Links },
  }
</script>

<style lang="scss" scoped>
.kkl-footer{
    background-color: #323237;
}
</style>