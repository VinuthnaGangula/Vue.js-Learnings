<template>
    <ul class="pa-2">
        <li v-for="item in items" :key="item.id">
            {{ item.name }}
        </li>
    </ul>
</template>

<script setup>
import { ref } from 'vue';

let items = ref([
    {id: 1, name: 'Python'},
    {id: 1, name: 'Java'},
    {id: 1, name: 'PHP'}
]);

</script>