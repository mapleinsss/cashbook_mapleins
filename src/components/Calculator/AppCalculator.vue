<template>
  <div v-show="showFlag">
    <p>{{result}}</p>

    <div @click="buttonEvent">
      <v-col cols="12">
        <v-row no-gutters>
          <v-col cols="3" class="float-right">
            <v-btn color="grey" block x-large tile class="mx-auto headline">隐藏</v-btn>
          </v-col>
        </v-row>
        <v-row no-gutters justify="center">
          <v-col cols="3">
            <v-btn color="grey" block x-large tile class="mx-auto headline">AC</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn color="grey" block x-large tile class="mx-auto headline">+/-</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn color="grey" block x-large tile class="mx-auto headline">%</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn color="orange" block x-large tile class="mx-auto headline">÷</v-btn>
          </v-col>
        </v-row>
        <v-row no-gutters>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">1</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">2</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">3</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn color="orange" block x-large tile class="mx-auto headline">*</v-btn>
          </v-col>
        </v-row>
        <v-row no-gutters justify="center">
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">4</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">5</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">6</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn color="orange" block x-large tile class="mx-auto headline">-</v-btn>
          </v-col>
        </v-row>
        <v-row no-gutters justify="center">
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">7</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">8</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">9</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn color="orange" block x-large tile class="mx-auto headline">+</v-btn>
          </v-col>
        </v-row>
        <v-row no-gutters justify="center">
          <v-col cols="6">
            <v-btn block x-large tile class="mx-auto headline">0</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn block x-large tile class="mx-auto headline">.</v-btn>
          </v-col>
          <v-col cols="3">
            <v-btn color="orange" block x-large tile class="mx-auto headline">=</v-btn>
          </v-col>
        </v-row>
      </v-col>
    </div>

  </div>
</template>

<script>
export default {
  name: 'AppCalculator',
  data () {
    return {
      result: 0,
      showFlag: true
    }
  },
  mounted () {},
  methods: {
    calculate: function (n1, operator, n2) {
      const firstValue = parseFloat(n1)
      const secondValue = parseFloat(n2)
      if (operator === 'add') return firstValue + secondValue
      if (operator === 'subtract') return firstValue - secondValue
      if (operator === 'multiply') return firstValue * secondValue
      if (operator === 'divide') return firstValue / secondValue
    },
    buttonEvent: function (event) {
      const key = event.target.textContent
      console.log(key)
    }
  }
}
</script>

<style scoped>
</style>
