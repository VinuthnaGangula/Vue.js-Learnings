<template>
    <div class="px-2">
        <p @click="update()">{{ message }}</p>
        <p>Count is {{ counter.count }}</p>
    </div>
</template>

<script setup>
import { reactive, ref } from 'vue';

const counter = reactive({
    count: 0
});

const message = ref('Some kind of text!');

function update() {
    message.value = "The text is now up-to-date!"
}
</script>

<style>
</style>