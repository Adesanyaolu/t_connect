
<script setup>
import { ref } from 'vue'

let text = ref('')

function onClick (){
    text.value = text
    console.log(text)
}

</script>


<template>

        <h1 class="text-3xl font-bold underline">
            Hello world!
        </h1>
       
            <input  placeholder="Type here">
            <button @click="onClick" >Submit</button>
            <p>{{ text }}</p>


</template>

<style>
p {
    color: red;
}

</style>