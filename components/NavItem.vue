<script setup lang="ts">
type Props = {
  to: string
}

const props = withDefaults(defineProps<Props>(), {
  to: ''
})
</script>

<template>
  <NuxtLink :to="props.to">
    <div class="font-md">
      <slot></slot>
    </div>
  </NuxtLink>
</template>
