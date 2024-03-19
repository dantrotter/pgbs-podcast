<template>
  <div class="wrapper">
    <p-header />
    <div class="layout">
      <div>
        <p-site-menu />
        <img src="~/static/Podbean_10000Downloads.png"/>
      </div>
      <div>
        <a href="https://www.youtube.com/watch?v=3z5Vi2vrnok">
          <img src="~/static/DT_mug_YouTubeThumbnail.png" class="YouTubeVideos" />
        </a>
        <div class="third-party-links">
          <p-podbean-links />
          <a href="https://www.youtube.com/channel/UCvdhN-S_y117F6p0V1nGR1Q/playlists"><img src="~/static/PlaylistButton.png" /></a>
        </div>
        <div class="quote">
            <p>This is the best full overview of the New Testament I have ever seen. I have been through Bible school, lived on the mission field for 18 years, did crusades, held pastors seminars, run medical clinics and started short-term Bible schools. Nobody tries to cover everything like PGBS does . . . PGBS really does a great job covering everything! 10 ⭐’s from me! – GG</p>
        </div>
      </div>
      <div>
        <ul class="benefit-bullets">
          <li>Podbean podcasts covering every verse of the <a href="https://dantrotter.podbean.com">NT</a> and <a href="https://pgbsoldtestament.podbean.com/">OT</a></li>
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
import PPodbeanLinks from '/components/PodbeanLinks.vue';

export default {
  name: 'IndexPage',
  components: { PHeader, PSiteMenu, PSocialShare, PPodbeanLinks },
  head() {
    return {
      title: "PGBS - Home"
    };
  }
}
</script>
