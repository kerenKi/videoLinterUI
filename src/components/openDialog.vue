<template>
  <div class="uploads">
    <form>
      <label for="chooseFile"> Or choose file to upload </label>
      <input type="file" id="chooseFile" @change="FileSelected" accept="video/*">
    </form>
  </div>
</template>
  
<script>

export default {
  name:'openDialog',
  methods:{
    FileSelected(event) {
      const file = event.target.files[0].path
      console.log(file)
      sendMessageToJulia(file)


      
    }
  }
}
</script>

<style scoped>
  .uploads{
    margin: auto;
    width: 50%;
  }
 input[type="file"]{
   display: none;
 }
  form {
  min-width: 400px;
  margin: 0 auto;
  padding: 20px;
}
form label{
  background-color: #7F9CCB;
  padding: 5px 10px;
  border-radius: 3px;
  font-size: 0.8rem;
  height: auto;
  border: 1px solid rgb(84, 82, 82);
}

form label:hover {
  background-color: #2D5BA3;
  color: white;
}

form label:active {
  background-color: #0D3F8F;
  color: white;
}
  
</style>

