<script lang="ts" setup>
const { data } = useFetch('https://ungh.cc/repos/unjs/nitro')

const { data: data2 } = useAsyncData('data', () => $fetch('https://ungh.cc/repos/unjs/nitro'))
</script>

<template>
  <div>
    {{ data }}
    {{ data2 }}
    <p>Custom Layout</p>
    <hr/>
    <slot />
  </div>
</template>
