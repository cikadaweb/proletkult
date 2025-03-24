<template>
  <main>
    <h1>Project {{ projectId }}</h1>
  </main>
</template>

<script setup lang="ts">
import { useRoute } from 'vue-router'

const route = useRoute()

const routeParams = route.params as {
  id: string
}
const projectId: string = routeParams.id
</script>
