<template>
  <!--    :value="value" 当前 tab 的 index -->
  <v-bottom-navigation
    color="primary"
    absolute
  >
    <v-btn to="account">
      <span>账户</span>
      <v-icon>fa fa-credit-card</v-icon>
    </v-btn>

    <v-btn to="record">
      <span class="orange--text">记一笔</span>
      <v-icon color="orange">fa fa-plus-square-o</v-icon>
    </v-btn>

    <v-btn to="setting">
      <span>设置</span>
      <v-icon>fa fa-gear</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
export default {
  name: 'BottomNav'
}
</script>

<style scoped>

</style>
