<template>
  <div>
      <input v-model="msg">
      <p>msg: {{msg}}</p>
      <p>computed msg: {{computedMsg}}</p>
      <button @click="greet">Greet</button>
  </div>
</template>
<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'
@Component
export default class App extends Vue {
  msg: number = 123;
  mounted () {
    this.greet()
  }
  get computedMsg (): string {
    return 'computed' + this.msg
  }
  greet (): void {
    alert('greeting: ' + this.msg)
  }
}
</script>
