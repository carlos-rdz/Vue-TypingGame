<template>
    <div>
    <ul class="list-group">
        <li class="list-group-item" v-for="word in words" >
            {{word}}
        </li>
    </ul>
    <button class="btn btn-primary" @click="deleteWords()"> delete word</button>
    </div>
</template>


<script>
export default {
    data(){
        return {
            words : ['this', 'is', 'easy']
        }
    },
    methods: {
        deleteWords(){
            this.words.pop()
        }
    }
}
</script>
