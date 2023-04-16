<template>
    <input class="pa-2" type="text" v-model="name" placeholder="Enter Name Here">
    <p class="pl-2 pt-2" v-if="savedName">Hi {{ savedName }}!</p>
    <br>
    <v-btn class="mr-1 my-1" @click="save()">Save</v-btn>
    <v-btn class="ml-1 my-1" @click="clear()">Clear</v-btn>
</template>

<script setup>
import { ref } from 'vue';

let name = ref('');
let savedName = ref('');

function save() {
    savedName.value = name.value;
    name.value = '';
}
function clear() {
    name.value = '';
    savedName.value = '';
}
</script>