<script lang="ts" setup>
const { data } = await useFetch('https://ungh.cc/repos/unjs/nitro')
</script>

<template>
  <div>
    {{ data }}
    <h1> About Page</h1>
    <NuxtLink to="/">Home</NuxtLink>
  </div>
</template>
