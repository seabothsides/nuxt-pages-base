<template lang="pug">
v-container
  v-row
    v-col.text-center.text-capitalize
      p.text-h2.blue-grey--text {{ more.title }}
  v-row
    v-col.text-center
      p.body-2 {{ more.description }}
  v-row
    v-col
      nuxt-content(:document='more')
</template>

<script>
export default {
  async asyncData({ $content }) {
    const more = await $content('pages/more').fetch()

    return { more }
  },
}
</script>
