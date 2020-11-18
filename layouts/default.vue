<template>
  <div>
    <Header />
    <div class="content-wrapper">
      <div class="content-divider-top">
        <svg
          data-name="Layer 1"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 1200 120"
          preserveAspectRatio="none"
        >
          <path
            d="M1200 120L0 16.48 0 0 1200 0 1200 120z"
            class="shape-fill"
          ></path>
        </svg>
      </div>
      <div class="content">
        <Nuxt />
      </div>
    </div>
  </div>
</template>
<script>
import Header from '~/components/Header.vue'
export default {
  components: { Header },
}
</script>
<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 18px;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

a {
  text-decoration: none;
  cursor: pointer;
}

.content-wrapper {
  @apply relative;
}

.content-divider-top {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
}

.content-divider-top svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 35px;
}

.content-divider-top .shape-fill {
  fill: #3d5a80;
}
</style>
