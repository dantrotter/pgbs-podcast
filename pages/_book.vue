<template>
  <div class="wrapper">
    <p-header />
    <div class="layout">
      <div>
        <p-site-menu />
      </div>
      <div>
        <p-book :name="this.$route.params.book" />
        <a href="https://dantrotter.podbean.com"><img src="~/static/AvailableOnPodbean.png" /></a>
      </div>
      <div>
        <p-social-share :title="title" :url="url" />
        <h2 class="small-header">Comments? Corrections?</h2>
        <a href="mailto:prettygoodbiblestudies@gmail.com">prettygoodbiblestudies@gmail.com</a>
      </div>
    </div>
  </div>
</template>

<script>
import PHeader from '/components/Header.vue';
import PBook from '/components/Book.vue';
import PSiteMenu from '/components/SiteMenu.vue';
import PSocialShare from '/components/SocialShare.vue';

export default {
  name: 'Book',
  components: { PHeader, PBook, PSiteMenu, PSocialShare },
  head() {
    return {
      title: this.title
    };
  },
  data() {
    return {
      title: "PGBS - " + this.$route.params.book.replace(/-/g, ' ').replace(/(^\w|\s\w)/g, w => w.toUpperCase()),
      url: 'url.com/' + this.$route.params.book
    }
  }
}
</script>