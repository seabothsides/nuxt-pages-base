<template lang="pug">
v-app
  v-app-bar(app, color='accent')
    v-btn(
      v-for='(i, id) in pageroute',
      :key='id',
      :to='i',
      text,
      active-class='info'
    ) {{ pagename[id] }}
  v-main
    nuxt
</template>

<script>
export default {
  data() {
    return {
      pageroute: ['/', 'about', 'more'],
      pagename: ['home', 'about', 'more add ons'],
    }
  },
}
</script>

<style lang="sass" scoped></style>
