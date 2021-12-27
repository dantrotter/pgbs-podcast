<template>
  <div class="wrapper">
    <p-header />
    <main>
      <p>Content</p>
    </main>
  </div>
</template>

<script>
import PHeader from '/components/Header.vue';

export default {
  name: 'IndexPage',
  components: { PHeader }
}
</script>