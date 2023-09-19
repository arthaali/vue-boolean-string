<script lang="ts" setup>
import TestComponent from "@/components/TestComponent.vue";

const value = ""
</script>

<template>
  <div class="App">
    <main >
   <TestComponent :value2="value" :value1="value"></TestComponent>
  </main>
    

  </div>
</template>

