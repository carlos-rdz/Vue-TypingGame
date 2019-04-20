<template>
<div>
      <div class="input-group mb-3">
        <div class="input-group-prepend">
          <span class="input-group-text" id="basic-addon1">Word</span>
        </div>
          <input type="text" class="form-control" v-model="word">
      </div>
    <div>{{word}}</div>  
</div>     
</template>


<script>
export default {  
  data(){
    return {
      word : ''
    }
  }
}

</script>




