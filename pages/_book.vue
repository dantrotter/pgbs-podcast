<template>
  <div>
    <p-menu />
    <p-book :name="this.$route.params.book" />
  </div>
</template>

<script>
import PMenu from '/components/Menu.vue';
import PBook from '/components/Book.vue';

export default {
  name: 'Book',
  components: { PMenu, PBook }
}
</script>
