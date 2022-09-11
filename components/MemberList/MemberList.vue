<script setup lang="ts">
const members = [
  { name: 'snowsphere', labels: ['producer', 'composer'] },
  { name: 'haco', labels: ['composer'] },
]
</script>

<template>
  <ul class="list-none">
    <MemberListItem
      v-for="item in members"
      :key="item.name"
      :name="item.name"
      :labels="item.labels"
    ></MemberListItem>
  </ul>
</template>
