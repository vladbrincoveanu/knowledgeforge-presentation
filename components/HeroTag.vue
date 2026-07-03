<template>
  <div class="hero-tag">
    <svg width="14" height="14" viewBox="0 0 28 28" fill="none" aria-hidden="true">
      <polygon points="14,2 26,8 26,20 14,26 2,20 2,8" stroke="#F6AE31" stroke-width="1.5" fill="none" />
      <circle cx="14" cy="14" r="2.5" fill="#F6AE31" />
      <line x1="14" y1="2" x2="14" y2="11.5" stroke="#F6AE31" stroke-width="1" opacity="0.6" />
      <line x1="14" y1="16.5" x2="14" y2="26" stroke="#F6AE31" stroke-width="1" opacity="0.6" />
      <line x1="2" y1="8" x2="11.5" y2="12.5" stroke="#F6AE31" stroke-width="1" opacity="0.6" />
      <line x1="16.5" y1="15.5" x2="26" y2="20" stroke="#F6AE31" stroke-width="1" opacity="0.6" />
      <line x1="26" y1="8" x2="16.5" y2="12.5" stroke="#F6AE31" stroke-width="1" opacity="0.6" />
      <line x1="11.5" y1="15.5" x2="2" y2="20" stroke="#F6AE31" stroke-width="1" opacity="0.6" />
    </svg>
    <span>KnowledgeForge</span>
  </div>
</template>

<style scoped>
.hero-tag {
  display: flex;
  width: fit-content;
  align-items: center;
  gap: 0.45rem;
  color: #F6AE31;
  font-family: var(--font-mono, 'Geist Mono', monospace);
  font-size: 0.62rem;
  font-weight: 600;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  margin-bottom: 0.6rem;
  opacity: 0.85;
}
</style>
