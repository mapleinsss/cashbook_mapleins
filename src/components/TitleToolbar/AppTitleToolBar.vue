<template>
  <v-row>
    <v-toolbar>
      <v-btn icon to="/index">
        <v-icon>mdi-arrow-left</v-icon>
      </v-btn>

      <v-toolbar-title>{{$route.meta.title}}</v-toolbar-title>
    </v-toolbar>
  </v-row>
</template>

<script>
export default {
  name: 'AppTitleToolBar'
}
</script>

<style scoped>

</style>
