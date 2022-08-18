<script setup>
const props = defineProps({
  label: {
    type: String,
    default: "На главную"
  }
});
</script>

<template>
  <a href="#" class="link" type="submit">{{ label }}</a>
</template>


<style lang="scss" scoped>
.link {
  font-weight: 700;
  font-size: 12px;
  line-height: 188.7%;
  letter-spacing: 0.07em;
  text-transform: uppercase;
  color: #1C85FE;
}
</style>


