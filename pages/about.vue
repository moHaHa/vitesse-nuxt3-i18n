<script setup lang="ts">
const online = useOnline()
</script>

<template>
  <div>
    <div>
      it's just a title -    <p>{{ $t('welcome') }}</p>
    </div>
  </div>
</template>
