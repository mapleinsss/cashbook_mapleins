<template>
  <div>
    <v-row>
      <v-toolbar flat>
        <v-btn icon to="/index" class="ml-1">
          <v-icon>mdi-arrow-left</v-icon>
        </v-btn>

        <v-toolbar-title>{{$route.meta.title}}</v-toolbar-title>
      </v-toolbar>
    </v-row>
    <v-divider class="mb-3"/>
  </div>
</template>

<script>
export default {
  name: 'AppTitleToolBar'
}
</script>

<style scoped>

</style>
