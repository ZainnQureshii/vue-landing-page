<template>
  <div class="services-section">
    <div class="services-section-inner">
      <div class="container">
        <MainHeading content="Premium services we offer" />
        <div class="text">
          With a global network in over 220 countries and territories across the
          globe, Our company is the most international company in the world and
          can offer solutions for an almost infinite number of logistics needs.
        </div>
        <ServicesContent />
        <div class="button">
          <Button content="Learn More About Our Services" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MainHeading from "../misc/MainHeadning";
import ServicesContent from "./ServicesContent";
import Button from "../misc/Button";
export default {
  name: "Services",
  components: {
    MainHeading,
    ServicesContent,
    Button
  }
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/_colors.scss";
.services-section {
  background: $section-background;
  padding: 50px 0;
  .services-section-inner {
    .text {
      margin: 20px 0;
      color: $light-gray-text;
    }
    .button {
      display: flex;
      justify-content: center;
    }
  }
}
</style>
