<template>
  <div class="wrapper">
    <p-header />
    <div class="layout">
      <div>
        <p-site-menu />
        <img src="~/static/Podbean_5000Downloads.png"/>
      </div>
      <div>
        <a href="https://www.youtube.com/watch?v=3z5Vi2vrnok">
          <img src="~/static/DT_mug_YouTubeThumbnail.png" class="YouTubeVideos" />
        </a>
        <div class="third-party-links">
          <a href="https://dantrotter.podbean.com"><img src="~/static/AvailableOnPodbean.png" /></a>
          <a href="https://www.youtube.com/channel/UCvdhN-S_y117F6p0V1nGR1Q/playlists"><img src="~/static/PlaylistButton.png" /></a>
        </div>
      </div>
      <div>
        <ul class="benefit-bullets">
          <li><a href="https://dantrotter.podbean.com">Podbean podcasts</a> covering every verse of the NT (OT is under construction)</li>
          <li><a href="https://www.youtube.com/channel/UCvdhN-S_y117F6p0V1nGR1Q/playlists">YouTube playlists</a> on five important theological topics</li>
            <ul>
              <li>Charismata</li>
              <li>Doctrines of Grace</li>
              <li>House Church Ecclesiology</li>
              <li>New Covenant Theology</li>
              <li>Orthodox Preterism</li>
            </ul>
          <li>Stream or download for free, ad-free</li>
          <li>Thousands of hours of research compiled into 40-minute audios</li>
          <li>High view of Scripture</li>
          <li>Sources used from many learned commentators of varied perspectives</li>
          <li>Character profiles, chronology, geography, textual variants, cross-Scriptural citations, theological and ethical problems, applications</li>
          <li>The perfect resource for any Bible teacher</li>
          <li>Nothing on the internet is like this</li>
        </ul>
        <p-social-share />
        <h2 class="small-header">Comments? Corrections?</h2>
        <a href="mailto:prettygoodbiblestudies@gmail.com">prettygoodbiblestudies@gmail.com</a>
        <hr>
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