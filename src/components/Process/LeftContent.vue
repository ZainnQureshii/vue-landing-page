<template>
  <div>
    <MainHeading content="Save time for the things that really matter" />
    <div class="text">
      We are now offering you the flexibility to integrate your business
      applications via APIs with our products and services.
    </div>
    <Button content="Get In Touch" />
  </div>
</template>

<script>
import MainHeading from "../misc/MainHeadning";
import Button from "../misc/Button";
export default {
  name: "LeftContent",
  components: {
    MainHeading,
    Button
  }
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/_colors.scss";
.text {
  margin: 20px 0;
  color: $light-gray-text;
}
</style>
