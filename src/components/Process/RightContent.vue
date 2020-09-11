<template>
  <div class="row">
    <div class="col-md-6">
      <div class="heading">1. Strategy</div>
      <div class="text">
        We provide one of the best services in this country for your products.
      </div>
    </div>
    <div class="col-md-6">
      <div class="heading">2. Input</div>
      <div class="text">
        We provide one of the best services in this country for your products.
      </div>
    </div>
    <div class="col-md-6">
      <div class="heading">3. Packaging</div>
      <div class="text">
        We provide one of the best services in this country for your products.
      </div>
    </div>
    <div class="col-md-6">
      <div class="heading">4. Delivery</div>
      <div class="text">
        We provide one of the best services in this country for your products.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "RightContent"
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/_colors.scss";
.row {
  > div {
    margin-bottom: 15px;
    .heading {
      margin-bottom: 10px;
      font-size: 20px;
      font-weight: 600;
      &:before {
        content: "";
        display: block;
        margin-top: 20px;
        margin-bottom: 10px;
        width: 40px;
        height: 3px;
        background: #000;
      }
    }
    .text {
      color: $light-gray-text;
      font-size: 15px;
    }
  }
}
</style>
