<template>
  <div class="resusable-button">
    <button>{{ content }}</button>
  </div>
</template>

<script>
export default {
  name: "Button",
  props: {
    content: String
  }
};
</script>

<style lang="scss" scoped>
.resusable-button {
  button {
    background: #d6010d;
    display: table;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    border: 0;
    outline: 0;
    color: #fff;
    font-weight: 550;
    padding: 10px 25px;
    border-radius: 3px;
  }
}

@media (max-width: 767px) {
  .resusable-button {
    button {
      font-size: 14px;
      padding: 7px 20px;
    }
  }
}
</style>
