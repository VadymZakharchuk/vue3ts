<template>
  <div class="app">
    <p> {{ name }} speaking...</p>
    <input type="text" v-model="iName">
    <button @click="changeName(iName)">Change</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App',
  components: {},
  data () {
    return {
      name: 'Vadym',
      age: 55 as string | number,
      iName: ''
    }
  },
  methods: {
    changeName (_name: string) {
      this.name = _name
    }
  }
})
</script>

<style>
</style>
