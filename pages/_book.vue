<template>
  <div class="wrapper">
    <p-header />
    <p-book :name="this.$route.params.book" />
  </div>
</template>

<script>
import PHeader from '/components/Header.vue';
import PBook from '/components/Book.vue';

export default {
  name: 'Book',
  components: { PHeader, PBook }
}
</script>