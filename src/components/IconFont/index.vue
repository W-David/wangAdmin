<template>
  <svg class="icon" aria-hidden="true">
    <use :xlink:href="`#${props.type}`"></use>
  </svg>
</template>

<script lang="ts">
export default { name: 'IzIconFont' };
</script>

<script setup lang="ts">
import type { PropType } from 'vue';
const props = defineProps({
  type: {
    type: [String, Number] as PropType<string | number>,
    default: ''
  }
});
</script>
