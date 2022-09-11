<script setup lang="ts">
const route = useRoute()

const pageName = computed(() => {
  let name = route.name

  if (typeof name === 'string') {
    name = name[0].toUpperCase() + name.slice(1).toLowerCase()
  }

  return name ?? ''
})
</script>

<template>
  <div v-if="pageName !== 'Index'">
    <div
      class="flex h-40 flex-wrap items-center border border-neutral-100 px-4 dark:border-neutral-700"
    >
      <h1
        class="inline-block p-2 text-4xl text-neutral-700 dark:text-neutral-200"
      >
        {{ pageName }}
      </h1>
    </div>
  </div>
</template>
