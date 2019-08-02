<template>
  <div class="uploads" id="drag-file" @mouseover="dropFile">
    <p>Drag your files here</p>
  </div>
</template>
  
<script>
export default {
  name:'dragAndDrop',
  methods:{
    dropFile(){
      var holder = document.getElementById('drag-file');

        holder.ondragover = () => {
            return false;
        };

        holder.ondragleave = () => {
            return false;
        };

        holder.ondragend = () => {
            return false;
        };

        holder.ondrop = (e) => {
            e.preventDefault();

            for (let f of e.dataTransfer.files) {
                console.log('File(s) you dragged here: ', f.path)
                sendMessageToJulia(f.path)
            }
            
            return false;
        };
    }
  }
}
</script>

<style scoped>
  .uploads{
    margin: auto;
    width: 50%;
  }
  #drag-file {
        background-color: rgb(97, 138, 155);
        color:white;
        text-align: center;
        width:300px;
        height:300px;
        margin: 10px;
        padding: 40px;
    }
</style>

