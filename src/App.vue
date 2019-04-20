<template>
  <div class="container">
    <div class="row">
      <app-header></app-header>
    </div>
    <div class="row">
      <app-word-display></app-word-display>
    </div>
    <div class="row">
      <app-word-input></app-word-input>
    </div>
  </div>
</template>


<script>
import Header from './components/Header.vue';
import wordDisplay from './components/wordDisplay.vue';
import wordInput from './components/wordInput.vue';

export default {
  data(){
    return {
      
    }
  },
  components : {
    appHeader : Header,
    appWordDisplay: wordDisplay,
    appWordInput: wordInput
  }
}
</script>


<style>

</style>
