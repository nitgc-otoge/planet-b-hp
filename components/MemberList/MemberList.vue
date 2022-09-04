<script setup lang="ts">
const members = [
  { name: 'snowsphere' },
  { name: 'haco' }
]
</script>

<template>
  <ul class="list-none">
    <MemberListItem v-for="item in members" :key="item.name" :name="item.name"></MemberListItem>
  </ul>
</template>