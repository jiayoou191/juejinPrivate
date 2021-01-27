<template>
  <div>
    <headerComponent />
    <footerComponent />
  </div>
</template>

<script>
import headerComponent from "./header/index"
import footerComponent from "./footer/index"
  export default {
    components: {
      headerComponent,
      footerComponent
    },
    
  }
</script>

<style lang="scss" scoped>

</style>