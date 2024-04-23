<script setup>
import TheWelcome from "../components/TheWelcome.vue";
import Dialog from "../components/Dialog.vue";
</script>

<template>
  <main>
    <TheWelcome />
    <button @click="$refs.dialog.open()">Test</button>

    <Dialog ref="dialog">
      <span>This is my dialog</span>
    </Dialog>
  </main>
</template>
