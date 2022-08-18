<script setup>
const props = defineProps({
  label: {
    type: String,
    default: 'Логин'
  },
  className: {
    type: String,
    default: "form__input"
  },
  for: {
    type: String,
    default: "user__login"
  }
});
</script>

<template>
  <label class="form_row__label" for="user__login">{{label}}</label>
</template>

<style lang="scss" scoped>
.btn {
  background: linear-gradient(93.76deg, #0568FF -27.36%, #31A0FD 121.33%);
  border-radius: 12px;
  font-weight: 700;
  font-size: 13px;
  line-height: 188.7%;
  text-align: center;
  letter-spacing: 0.07em;
  text-transform: uppercase;
  color: #FFFFFF;
  padding: 16px;
  min-width: 270px;
}
</style>



