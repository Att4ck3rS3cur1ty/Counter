<template>
  <div>
    <h3>TS Counter</h3>
    <div>{{count}} is {{isOdd}}</div>
    <div>
      <button @click="increment()">INCREMENT</button>
    </div>
  </div>
</template>

<script lang="ts">
import * as Vue from 'vue'
import Component from 'vue-class-component'

@Component
export default class Counter extends Vue{ 
  count = 0
  increment(){this.count++}
  get isOdd(){
    return (this.count % 2 === 0)? 'even': 'odd'
  }
}
</script>
