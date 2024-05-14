<template>
  <div id="app">
  <button @click="count++">
    Count is: {{ count }}
  </button>
</div>
 
</template>

<script>
import { createApp, ref } from 'vue'

createApp({
  setup() {
    return {
      count: ref(0)
    }
  }
}).mount('#app')
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

button{
  width: 100px;
  border-color: transparent;
  border-radius: 10px;
  background-color: aqua;
  color:red;
}
</style>
