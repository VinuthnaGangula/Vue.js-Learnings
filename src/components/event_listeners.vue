<template>
    <v-btn @click="increment()">Count is: {{ count }}</v-btn>
</template>

<script setup>
import { ref } from 'vue';

let count = ref(0);

function increment() {
    count.value++;
}
</script>