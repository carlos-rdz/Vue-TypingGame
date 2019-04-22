<template>
  <div class="container">
    <div class="row top-buffer">
      <app-header></app-header>
    </div>
    <div class="row top-buffer">
      <app-word-display 
        :ourWords="words"
        :deleteWord="deleteWord"
        >
        
      </app-word-display>
    </div>
    <div class="row top-buffer">
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
      words : ['this', 'is', 'easy']
    }
  },
  components : {
    appHeader : Header,
    appWordDisplay: wordDisplay,
    appWordInput: wordInput
  },
  methods : {
    deleteWord(){
      this.words.pop()
    }
  }
}
</script>


<style>
.top-buffer { margin-top:20px; }
</style>
