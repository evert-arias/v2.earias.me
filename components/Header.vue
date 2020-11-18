<template>
  <nav>
    <div class="nav-left-section">
      <div class="nav-logo"></div>
    </div>
    <ul class="nav-right-section">
      <li><a href="#">Apps</a></li>
      <li><a href="#">Projects</a></li>
      <li><a href="#">Blog</a></li>
      <li><a href="#">Github</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Thanks</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped>
nav {
  @apply bg-primary-500 w-full h-16 flex justify-end;
}

nav .nav-left-section {
  @apply mr-auto h-auto w-auto flex items-center;
}

nav .nav-left-section .nav-logo {
  background-image: url('../assets/logo.svg');
  @apply w-10 h-10 mr-auto ml-3 bg-no-repeat bg-center;
}

nav .nav-right-section {
  @apply w-auto h-auto flex list-none justify-center items-center mr-2;
}

nav .nav-right-section a {
  @apply text-secondary-300 text-base mr-4;
}

nav .nav-right-section a:hover {
  @apply text-primary-700;
}
</style>
