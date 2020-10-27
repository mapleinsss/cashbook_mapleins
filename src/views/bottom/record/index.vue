<template>
  <div>
    <app-title-tool-bar/>
    <app-calculator/>
  </div>
</template>

<script>
import AppTitleToolBar from '@/components/TitleToolbar/AppTitleToolBar'
import AppCalculator from '@/components/Calculator/AppCalculator'
export default {
  name: 'Record',
  components: { AppCalculator, AppTitleToolBar }
}
</script>

<style scoped>

</style>
