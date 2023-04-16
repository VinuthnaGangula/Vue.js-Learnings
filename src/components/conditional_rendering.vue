<template>
    <span class="pa-2">{{ message }}</span>
    <v-btn class="pa-2" @click="toggle()">Toggle</v-btn>
</template>

<script setup>
import { ref } from 'vue';

let message = ref('Hi!');

function toggle() {
    if (message.value == 'Hi!')
        message.value = 'Bye!';
    else
        message.value = 'Hi!';
}
</script>