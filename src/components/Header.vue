<template>
  <div class="header">
    <div class="header-inner">
      <div class="logo-block">
        <img src="../assets/images/logo.png" alt="logo" />
      </div>
      <div class="nav-block">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Pricing</a></li>
          <li><a href="#">FAQs</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </div>
      <div class="responsive-nav">
        <div></div>
        <div></div>
        <div></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header {
  position: absolute;
  width: 100%;
  z-index: 1;
  .header-inner {
    display: flex;
    justify-content: space-between;
    padding: 30px 50px;
    .logo-block {
      img {
        width: 250px;
      }
    }
    .nav-block {
      ul {
        list-style: none;
        display: flex;
        margin-bottom: 0;
        li {
          padding: 10px 20px;
          a {
            font-weight: 550;
            font-size: 17px;
            color: #fff;
          }
        }
      }
    }
  }
}
@media (min-width: 992px) {
  .responsive-nav {
    display: none;
  }
}
@media (max-width: 991px) {
  .nav-block {
    display: none;
  }
  .responsive-nav {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    > div {
      width: 25px;
      height: 3px;
      background: #fff;
      &:not(:last-child) {
        margin-bottom: 5px;
      }
    }
  }
}

@media (max-width: 575px) {
  .header {
    .header-inner {
      padding: 30px 15px;
      .logo-block {
        img {
          width: 170px;
        }
      }
    }
  }
}
</style>
