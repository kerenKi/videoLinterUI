<template>
  <div id="app">
    <uploadFile />
  </div>
</template>

<script>
import uploadFile from './components/uploadFile'

export default {
  name: 'app',
  components: {
    uploadFile
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin:auto;
  background-color: rgba(114, 186, 249, 0.845);
}
</style>
