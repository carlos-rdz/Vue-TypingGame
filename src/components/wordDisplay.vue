<template>
    <ul class="list-group">
        <li class="list-group-item" v-for="(word, key, index) in words" v-if="word">
            {{index + 1}}: {{key}}
        </li>
    </ul>
</template>


<script>
export default {
    data(){
        return {
            words : {
                this : true,
                is: true,
                easy: true
            }
        }
    }
}
</script>
