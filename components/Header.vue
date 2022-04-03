<template>
  <header>
    <NuxtLink to="/" class="logo">
      <img src="~/static/PGBS.svg" /> <h1>Pretty Good Bible Studies</h1>
    </NuxtLink>
    <p-bible-menu />
  </header>
</template>

<script>
  import PBibleMenu from '/components/BibleMenu.vue';

  export default {
    name: 'Header',
    components: { PBibleMenu }
  }
</script>