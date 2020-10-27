<template>
  <div>
    <v-row dense>
      <v-col cols="12">
        <v-card dark>
          <v-card-title class="headline pb-0">
            <div class="blue--text display-2 mr-2">10</div>月 · 支出
          </v-card-title>
          <v-card-title class="display-1 pt-1">
            3049
          </v-card-title>
          <v-card-subtitle>本月收入 34020.10</v-card-subtitle>
        </v-card>
      </v-col>
      <v-col cols="12">
        <v-card flat>
          <v-list-item three-line @click="doClick">
            <v-list-item-avatar>
              <v-icon class="float-left" color="red">fa fa-credit-card</v-icon>
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title class="title">
                <div class="float-left">今天</div>
                <div class="float-right red--text">+ 95</div>
              </v-list-item-title>
              <v-list-item-title class="title">
                <v-list-item-subtitle class="float-left">还没有记过账</v-list-item-subtitle>
                <div class="float-right green--text">- 50</div>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-divider/>
        </v-card>
      </v-col>
      <v-col cols="12">
        <v-card flat>
          <v-list-item three-line>
            <v-list-item-avatar>
              <v-icon class="float-left" color="red">fa fa-credit-card</v-icon>
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title class="title">
                <div class="float-left">本周</div>
                <div class="float-right red--text">+ 302</div>
              </v-list-item-title>
              <v-list-item-title class="title">
                <v-list-item-subtitle class="float-left">10月26日 - 11月11日</v-list-item-subtitle>
                <div class="float-right green--text">- 892</div>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-divider/>
        </v-card>
      </v-col>
      <v-col cols="12">
        <v-card flat>
          <v-list-item three-line>
            <v-list-item-avatar>
              <v-icon class="float-left" color="red">fa fa-credit-card</v-icon>
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title class="title">
                <div class="float-left">10 月</div>
                <div class="float-right red--text">+ 103</div>
              </v-list-item-title>
              <v-list-item-title class="title">
                <v-list-item-subtitle class="float-left">10月1日 - 10月31日</v-list-item-subtitle>
                <div class="float-right green--text">- 332</div>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-divider/>
        </v-card>
      </v-col>
      <v-col cols="12">
        <v-card flat>
          <v-list-item three-line>
            <v-list-item-avatar>
              <v-icon class="float-left" color="red">fa fa-credit-card</v-icon>
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title class="title">
                <div class="float-left">本年</div>
                <div class="float-right red--text">+ 239290</div>
              </v-list-item-title>
              <v-list-item-title class="title">
                <v-list-item-subtitle class="float-left">2020年</v-list-item-subtitle>
                <div class="float-right green--text">- 93832</div>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-divider/>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'index',
  methods: {
    doClick () {
      console.log('点击 list-item ')
    }
  }
}
</script>

<style scoped>

</style>
