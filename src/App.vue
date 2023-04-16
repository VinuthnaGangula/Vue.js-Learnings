<template>
  <v-app>
    <v-main class="pa-4">
      <div class="section">
        <h1>Declarative Rendering</h1>
        <declarative_rendering />
      </div>
      
      <div>
        <h1>Attribute Binding</h1>
        <attribute_binding />
      </div>

      <div>
        <h1>Event Listeners</h1>
        <event_listeners />
      </div>

      <div>
        <h1>Form Bindings</h1>
        <form_bindings />
      </div>

      <div>
        <h1>Conditional Rendering</h1>
        <conditional_rendering />
      </div>

      <div>
        <h1>List Rendering</h1>
        <list_rendering />
      </div>
    </v-main>
  </v-app>
</template>

<script setup>
import declarative_rendering from './components/declarative_rendering.vue';
import attribute_binding from './components/attribute_binding.vue';
import event_listeners from './components/event_listeners.vue';
import form_bindings from './components/form_bindings.vue';
import conditional_rendering from './components/conditional_rendering.vue';
import list_rendering from './components/list_rendering.vue';
</script>

<style scoped>
.section {
  padding: 4px;
}
</style>