<script setup lang="ts">
const links = [
  {
    name: 'Bandcamp',
    url: 'https://aoi-wakusei.bandcamp.com/',
  },
  {
    name: 'SoundCloud',
    url: 'https://soundcloud.com/planet_b_bms',
  },
]
</script>

<template>
  <ul>
    <LinkListItem
      v-for="item in links"
      :key="item.name"
      :name="item.name"
      :url="item.url"
    ></LinkListItem>
  </ul>
</template>
