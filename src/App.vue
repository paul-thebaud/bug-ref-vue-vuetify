<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import { ref } from 'vue';
import HelloWorld from './components/HelloWorld.vue'

const inputRef = ref(null);

const onLogRef = () => {
  console.log(inputRef.value);
  console.log((inputRef.value as any).validate);
}
</script>

<template>
<v-app>
  <v-main>
    <v-container>
      <v-text-field ref="inputRef" label="Test input" />
      <v-btn @click="onLogRef">
        Log ref content
      </v-btn>
    </v-container>
  </v-main>
</v-app>
</template>
