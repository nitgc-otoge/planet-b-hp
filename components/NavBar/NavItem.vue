<script setup lang="ts">
type Props = {
  to: string
  icon: string
}

const props = withDefaults(defineProps<Props>(), {
  to: '',
  icon: ''
})
</script>

<template>
  <NuxtLink :to="props.to">
    <div class="">
      <span class="material-icons-round text-3xl text-neutral-300 hover:text-blue-800 transition">
        {{ props.icon }}
      </span>
    </div>
  </NuxtLink>
</template>
