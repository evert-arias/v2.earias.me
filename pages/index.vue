<template>
  <div>
    <section>
      <Hero />
    </section>
    <section>
      <Apps />
    </section>
    <section>
      <Projects />
    </section>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Hero from '~/components/Hero.vue'
import Apps from '~/components/Apps.vue'
import Projects from '~/components/Projects.vue'
export default Vue.extend({
  components: { Hero, Apps, Projects },
})
</script>

<style></style>
