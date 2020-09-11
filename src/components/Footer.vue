<template>
  <div>
    <div class="footer">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-3">
            <div class="logo-block">
              <img src="../assets/images/footer-logo.png" alt="footer-logo" />
            </div>
          </div>
          <div class="col-sm-6 col-md-3">
            <div class="heading">Learn More</div>
            <ul>
              <li><a href="#">About Us</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Contact Us</a></li>
              <li><a href="#">FAQs</a></li>
              <li><a href="#">Support</a></li>
            </ul>
          </div>
          <div class="col-sm-6 col-md-3">
            <div class="heading">Services</div>
            <ul>
              <li><a href="#">Job Board</a></li>
              <li><a href="#">Buy Sell/Lease</a></li>
              <li><a href="#">Marketplace</a></li>
              <li><a href="#">Finance/Accounting</a></li>
              <li><a href="#">Insurance</a></li>
            </ul>
          </div>
          <div class="col-sm-6 col-md-3">
            <div class="heading">Quick Links</div>
            <ul>
              <li><a href="#">Terms Of Services</a></li>
              <li><a href="#">Privacy policy</a></li>
              <li><a href="#">Sitemap</a></li>
              <li><a href="#">Sign In</a></li>
              <li><a href="#">Sign Up</a></li>
            </ul>
          </div>
        </div>
        <div class="bottom-footer">
          <div class="copyright">
            All Rights Reserved&copy; 2020
          </div>
          <div class="social-links">
            <ul>
              <li>
                <a href="#">
                  <img src="../assets/images/twitter.svg" alt="social-icon" />
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="../assets/images/facebook.svg" alt="social-icon" />
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="../assets/images/linkedin.svg" alt="social-icon" />
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style lang="scss" scoped>
@import "../assets/styles/_colors.scss";
.footer {
  .row {
    padding: 50px 0;
    .logo-block {
      display: table;
      margin: auto;
      position: relative;
      top: 50%;
      transform: translateY(-50%);
      img {
        width: 160px;
      }
    }
    .heading {
      margin-bottom: 8px;
      font-weight: 550;
    }
    ul {
      margin-top: 10px;
      list-style: none;
      margin: 0;
      padding: 0;
      li {
        margin-bottom: 5px;
        position: relative;
        padding-left: 15px;
        display: flex;
        align-items: center;
        transition: 300ms all;
        &:before {
          content: "";
          margin-top: -2px;
          position: absolute;
          display: block;
          width: 6px;
          height: 6px;
          border-right: 1px solid $light-gray-text;
          border-bottom: 1px solid $light-gray-text;
          top: 50%;
          left: 0;
          transform: rotate(-45deg) translateY(-50%);
        }
        &:hover {
          margin-left: 7px;
        }
        a {
          color: $light-gray-text;
          font-size: 15px;
          text-decoration: none;
        }
      }
    }
  }
  .bottom-footer {
    padding: 20px 0;
    border-top: 1px solid #ccc;
    display: flex;
    justify-content: space-between;
    .copyright {
      color: $light-gray-text;
    }
    .social-links {
      ul {
        list-style: none;
        margin: 0;
        padding: 0;
        display: flex;
        li {
          padding: 0 5px;
          a {
            img {
              width: 20px;
              height: 20px;
            }
          }
        }
      }
    }
  }
}

@media (max-width: 767px) {
  .row {
    > div {
      margin-bottom: 30px;
    }
  }
}
@media (max-width: 575px) {
  .row {
    > div {
      position: relative;
      left: 50%;
      transform: translateX(-50%);
    }
  }

  .bottom-footer {
    flex-direction: column;
    align-items: center;
    .copyright {
      order: 2;
      margin-top: 18px;
    }
  }
}
</style>
