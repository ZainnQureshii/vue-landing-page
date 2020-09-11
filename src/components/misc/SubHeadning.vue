<template>
  <h2>{{ content }}</h2>
</template>

<script>
export default {
  name: "SubHeading"
};
</script>

<style lang="scss" scoped>
h1 {
  font-size: 36px;
  font-weight: 600;
  &:after {
    content: "";
    display: block;
    background: $theme-color;
    width: 50px;
    height: 5px;
    margin-top: 20px;
  }
}
</style>
