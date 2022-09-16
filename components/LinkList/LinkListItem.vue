<script setup lang="ts">
type Props = {
  name: string
  url: string
}

const props = withDefaults(defineProps<Props>(), {
  name: '',
  url: ''
})

</script>

<template>
  <li>
    <a :href="props.url" target="_blank" class="">{{ props.name }}</a>
  </li>
</template>