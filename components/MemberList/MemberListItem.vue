<script setup lang="ts">
type LinkItem = {
  title: string
  icon?: string
  url: string
}

type Props = {
  name: string
  links?: LinkItem[]
}

const props = withDefaults(defineProps<Props>(), {})
</script>

<template>
  <li class="py-2">
    <h3 class="font-semibold">{{ props.name }}</h3>
  </li>
</template>
