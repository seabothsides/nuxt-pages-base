<template lang="pug">
v-container
  v-row
    v-col.text-center.text-capitalize
      p.text-h1.blue-grey--text {{ index.title }}
  v-row
    v-col.text-center
      p.body-1 {{ index.description }}
  v-row
    v-col
      nuxt-content(:document='index')
</template>

<script>
export default {
  async asyncData({ $content }) {
    const index = await $content('index').fetch()

    return { index }
  },
}
</script>
