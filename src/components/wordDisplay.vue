<template>
    <div>
    <ul class="list-group">
        <li class="list-group-item" v-for="word in ourWords" >
            {{word}}
        </li>
    </ul>
    <button class="btn btn-primary" @click="deleteWord"> delete word</button>
    </div>
</template>


<script>
export default {
    data(){
        return {
            
        }
    },
    methods: {

    },
    props : ['ourWords','deleteWord']
}
</script>
