<template>
  <div id="app">
    <dragAndDrop />
    <openDialog />
  </div>
</template>

<script>
import openDialog from './components/openDialog'
import dragAndDrop from './components/dargAndDrop'

export default {
  name: 'app',
  components: {
    dragAndDrop,
    openDialog
  }
}
</script>

<style>
body{
  margin:auto;
  background-color: rgba(114, 186, 249, 0.845);
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  font-size: 20px;
  font-weight: 600;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin:auto;
}
</style>
