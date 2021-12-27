<template>
  <header>
    <NuxtLink to="/">PGBS</NuxtLink>
    <p-menu />
  </header>
</template>

<script>
  import PMenu from '/components/Menu.vue';

  export default {
    name: 'Header',
    components: { PMenu }
  }
</script>