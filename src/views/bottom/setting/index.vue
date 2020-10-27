<template>
  <div>
    <app-title-tool-bar/>
    <v-row justify="center" class="mb-2">
      <v-avatar size="46">
        <img src="http://img.mapleins.cn/avatar1.jpg" alt="https://cdn.jsdelivr.net/gh/mapleinsss/mapleins_blog_cdn@master/images/headers/unknownheader.jpg"/>
      </v-avatar>
    </v-row>
    <v-row justify="center" class="mb-2">
      <p class="headline">抱有远大理想的胡</p>
    </v-row>
    <v-row no-gutters>
      <v-col cols="12">
        <v-card flat>
          <v-list dense>
            <!--v-model="model"-->
            <v-list-item-group>
              <v-list-item>
                <v-list-item-icon>
                  <v-icon>fa fa-credit-card</v-icon>
                </v-list-item-icon>
                <v-list-item-content>
                  <v-list-item-title>账户设置</v-list-item-title>
                </v-list-item-content>
              </v-list-item>
              <v-divider/>
              <v-list-item>
                <v-list-item-icon>
                  <v-icon>fa fa-credit-card</v-icon>
                </v-list-item-icon>
                <v-list-item-content>
                  <v-list-item-title>关于</v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import AppTitleToolBar from '@/components/TitleToolbar/AppTitleToolBar'
export default {
  name: 'Setting',
  components: { AppTitleToolBar },
  methods: {
    doClick () {
      console.log('1')
    }
  }
}
</script>

<style scoped>

</style>
