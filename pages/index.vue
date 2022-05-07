<template>
  <div class="wrapper">
    <p-header />
    <div class="layout">
      <div>
        <p-site-menu />
      </div>
      <div>
        <amp-youtube
          data-videoid="3z5Vi2vrnok"
          layout="responsive"
          width="480"
          height="270"
        ></amp-youtube>
      </div>
      <div>
        <ul class="benefit-bullets">
          <li>Stream or download for free, ad-free</li>
          <li>Thousands of hours of research compiled into 40-minute audios</li>
          <li>High view of Scripture</li>
          <li>Sources used from many learned commentators of varied perspectives</li>
          <li>Character profiles, chronology, geography, textual variants, cross-Scriptural citations, theological and ethical problems, applications</li>
          <li>The perfect resource for any Bible teacher</li>
          <li>Nothing on the internet is like this</li>
          <li>Test</li>
        </ul>
        <p-social-share />
        <h2 class="small-header">Comments? Corrections?</h2>
        <a href="mailto:prettygoodbiblestudies@gmail.com">prettygoodbiblestudies@gmail.com</a>
        <hr>
        <a href="https://dantrotter.podbean.com"><img src="~/static/AvailableOnPodbean.png" /></a>
      </div>
    </div>
  </div>
</template>

<script>
import PHeader from '/components/Header.vue';
import PSiteMenu from '/components/SiteMenu.vue';
import PSocialShare from '/components/SocialShare.vue';

export default {
  name: 'IndexPage',
  components: { PHeader, PSiteMenu, PSocialShare },
  head() {
    return {
      title: "PGBS - Home"
    };
  }
}
</script>