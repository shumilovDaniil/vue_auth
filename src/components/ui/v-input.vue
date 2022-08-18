<script setup>
const props = defineProps({
  placeholder: {
    type: String,
    default: "Введите логин"
  },
  className: {
    type: String,
    default: "form__input"
  },
  name: {
    type: String,
    default: "user__login"
  },
  type: {
    type: String,
    default: "text"
  }
});
</script>

<template>
  <input v-bind:class="className" v-bind:name="name" v-bind:type="type" v-bind:placeholder="placeholder"/>
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



