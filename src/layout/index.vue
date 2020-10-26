<template>
  <div>
    <app-main/>
    <app-snackbar/>
    <bottom-nav/>
  </div>
</template>

<script>
import AppMain from './components/AppMain'
import AppSnackbar from '../components/Snackbar/AppSnackbar'
import BottomNav from './components/BottomNav/index'
export default {
  name: 'Layout',
  components: { BottomNav, AppSnackbar, AppMain }
}
</script>

<style scoped>

</style>
