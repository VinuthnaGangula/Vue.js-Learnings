<template>
    <div>
        <p :class="titleClass">This is a red colored sentence.</p>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const titleClass = 'title';
</script>

<style scoped>
.title {
    color: red;
}
</style>