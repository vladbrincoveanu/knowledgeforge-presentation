<script setup>
import { computed } from 'vue'
import { useSlideContext } from '@slidev/client'
const { $frontmatter: fm } = useSlideContext()
const showGlow = computed(() => fm.glow !== false)
</script>

<template>
  <div class="slidev-layout l-cover">
    <SlideBg />
    <div v-if="showGlow" class="glow" />
    <Reveal class="l-center">
      <Fit>
        <HeroTag />
        <div v-if="fm.kicker" class="kicker">{{ fm.kicker }}</div>
        <h1 class="fs-cover mw-cover" v-html="fm.title" />
        <div v-if="fm.subtitle" class="fs-lead mw-lead dim mt-5" v-html="fm.subtitle" />
        <slot />
      </Fit>
    </Reveal>
    <Foot :mark="false" />
  </div>
</template>
