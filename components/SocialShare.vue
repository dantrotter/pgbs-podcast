<template>
<div class="social-share">
  <h2 class="small-header">Share</h2>
  <ul>
    <li>
      <amp-social-share
        type="facebook"
        aria-label="Share on Facebook"
        width="20"
        height="20"
      ></amp-social-share>
    </li>
    <li>
      <amp-social-share
        type="twitter"
        aria-label="Share on Twitter"
        width="20"
        height="20"
      ></amp-social-share>
    </li>
    <li>
      <amp-social-share
        type="parler"
        data-share-endpoint="https://parler.com/new-post"
        :data-param-message="encodeURIComponent(title)"
        :data-param-url="encodeURIComponent(url)"
        width="20"
        height="20"
        aria-label="Share on Parler"
      >
        <img src="~/static/social/parler.svg" alt="Parler" />
      </amp-social-share>
    </li>
    <li>
      <amp-social-share
        type="gettr"
        data-share-endpoint="https://parler.com/new-post"
        :data-param-text="encodeURIComponent(title)"
        :data-param-url="encodeURIComponent(url)"
        width="20"
        height="20"
        aria-label="Share on Parler"
      >
        <img src="~/static/social/gettr.png" alt="Gettr" />
      </amp-social-share>
    </li>
    <li>
      <a :href="`mailto:?subject=${encodeURIComponent(title)}&body=${encodeURIComponent(url)}`">
      <svg width="22" height="20" viewBox="0 0 22 20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <rect x="2" y="1" width="18" height="18" stroke="#AAAAAA" stroke-width="2"/>
        <path d="M20.5 4.80518L11.4351 10.5L1.5 3.93506" stroke="#AAAAAA" stroke-width="2"/>
      </svg>
      </a>
    </li>
  </ul>
  </div>
</template>

<script>
  export default {
    name: 'PSocialShare',
    props: {
      url: {
        type: String,
        default: 'url.com'
      },
      title: {
        type: String,
        default: 'PGBS - Home'
      }
    }
  }
</script>