<script setup lang="ts">
const { locale } = useI18n()

function toggleLang() {
  locale.value = locale.value === 'ar' ? 'en' : 'ar'
}
</script>

<template>
  <div>
    <button class="!outline-none" @click="toggleLang">
      <div class="i-carbon-language" /> {{ locale }}
    </button>
    <p>{{ $t('welcome') }}</p>
  </div>
</template>

<style>
html,
body,
#__nuxt {
  height: 100vh;
  margin: 0;
  padding: 0;
}

html.dark {
  background: #222;
  color: white;
}
</style>
