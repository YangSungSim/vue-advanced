<template>
  <div id="app">
      <check-box v-model="checked"></check-box>
      <fetch-data url="https://jsonplaceholder.typicode.com/users/i"></fetch-data>
  </div>
</template>

<script>
import CheckBox from './components/CheckBox.vue'
import FetchData from "./components/FetchData";

export default {
  name: 'App',
  components: {
      FetchData,
    CheckBox
  },
  data() {
    return {
      checked:false
    }
  }
}
</script>

<style>

</style>
