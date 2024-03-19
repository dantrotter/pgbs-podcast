<template>
  <nav class="site-menu">
    <ul>
      <li><NuxtLink to="/about">About Dan Trotter</NuxtLink></li>
      <li><NuxtLink to="/doctrinal-statement">Doctrinal Statement</NuxtLink></li>
      <li><NuxtLink to="/doctrinal-distinctives">Doctrinal Distinctives</NuxtLink></li>
      <li><NuxtLink to="/sources">Sources Used</NuxtLink></li>
      <li><NuxtLink to="/target-audience">Target Audience</NuxtLink></li>
      <li><NuxtLink to="/modus-operandi">Modus Operandi</NuxtLink></li>
      <li><NuxtLink to="/controversial-passages">Controversial Passages</NuxtLink></li>
    </ul>
  </nav>
</template>

<script>
  export default {
    name: 'PSiteMenu'
  }
</script>