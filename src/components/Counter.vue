<template>
  <div>
    <h3>JS Counter</h3>
    <div>{{count}} is {{isOdd}}</div>
    <div>
      <button @click="increment()">INCREMENT</button>
    </div>
  </div>
</template>

<script lang="js">
  export default{
    data(){
      return {
        count: 0
      }
    },
    methods: {
      increment(){
        this.count++
      }
    },
    computed: {
      isOdd(){
        return (this.count % 2 === 0) ? 'even': 'odd'
      }
    }
  }
</script>
