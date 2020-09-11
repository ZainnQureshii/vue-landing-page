<template>
  <div class="newsletter">
    <div class="newsletter-inner">
      <div class="container">
        <div class="heading">Subscribe to our newsletter</div>
        <div class="subscribe">
          <input
            class="form-control"
            type="text"
            placeholder="Enter your email"
          />
          <Button content="Subscribe" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "./misc/Button";
export default {
  name: "NewsLetter",
  components: {
    Button
  }
};
</script>

<style lang="scss" scoped>
.newsletter {
  background: url("../assets/images/newsletter-bg.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  padding: 60px 0;
  .heading {
    color: #fff;
    font-size: 36px;
    font-weight: 600;
    text-transform: capitalize;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.8);
  }
  .subscribe {
    display: flex;
    align-items: center;
    margin-top: 15px;
    max-width: 600px;
    input {
      margin-right: 10px;
      padding: 20px 10px;
      border-radius: 3px;
    }
  }
}

@media(max-width: 575px) {
  .newsletter {
    .heading {
      font-size: 28px;
    }
    .subscribe {
      flex-direction: column;
      input {
        font-size: 14px;
        padding: 10px 8px;
        margin-bottom: 20px;
      }
    }
  }
}
</style>
