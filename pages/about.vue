<template lang="pug">
v-container
  v-row
    v-col.text-center.text-capitalize
      p.text-h2.blue-grey--text {{ about.title }}
  v-row
    v-col.text-center
      p.body-2 {{ about.description }}
  v-row
    v-col
      nuxt-content(:document='about')
</template>

<script>
export default {
  async asyncData({ $content }) {
    const about = await $content('pages/about').fetch()

    return { about }
  },
}
</script>
