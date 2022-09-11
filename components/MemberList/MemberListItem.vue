<script setup lang="ts">
type LinkItem = {
  title: string
  icon?: string
  url: string
}

type Props = {
  name: string
  labels: string[]
  links?: LinkItem[]
}

const props = withDefaults(defineProps<Props>(), {})
</script>

<template>
  <li class="mb-4 rounded-md py-4 px-4">
    <h3 class="font-semibold">{{ props.name }}</h3>
    <div>
      <span v-for="(label, index) in props.labels" :key="label">
        {{ label }}<span v-if="props.labels.length > 1 && index !== props.labels.length - 1">,</span>&nbsp;
      </span>
    </div>
  </li>
</template>
