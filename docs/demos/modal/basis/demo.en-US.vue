<template>
  <Button type="primary" @click="active = !active">
    Open
  </Button>
  <Modal
    v-model:active="active"
    transfer
    title="Title"
    :width="500"
  >
    <p>Some Content</p>
    <p>Some Content</p>
    <p>Some Content</p>
  </Modal>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const active = ref(false)
</script>
