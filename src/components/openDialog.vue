<template>
  <div class="uploads">
    <p id="SelectFile" @click="openDialog">Or upload a file from here</p>
  </div>
</template>
  
<script>

export default {
  name:'openDialog',
  methods:{
    openDialog(){
      console.log('test')
    }
  }
}
</script>

<style scoped>
  .uploads{
    margin: auto;
    width: 50%;
  }
  #SelectFile {
    margin: 20px;
    color: rgba(4, 116, 164, 0.673);
  }
  #SelectFile:hover{
    cursor: pointer;
    color: white;
  }
  
</style>

