<template>
  <h1>{{ content }}</h1>
</template>

<script>
export default {
  name: "MainHeading",
  props: {
    content: String
  }
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/_colors.scss";
h1 {
  font-size: 36px;
  font-weight: 600;
  text-transform: capitalize;
  &:after {
    content: "";
    display: block;
    background: $theme-color;
    width: 70px;
    height: 5px;
    margin-top: 20px;
  }
}
@media (max-width: 767px) {
  h1 {
    font-size: 28px;
    &:after {
      height: 4px;
    }
  }
}
</style>
