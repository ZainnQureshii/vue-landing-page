<template>
  <div class="hero-section">
    <div class="background">
      <div class="container">
        <div class="content">
          <div class="main-content">
            <div class="text">
              <div class="main-text">We Deliver With Speed</div>
              <div class="sub-text">
                Express courier delivery from the specialists in international
                shipping.
              </div>
            </div>
            <div class="button">
              <button>Talk To Us</button>
            </div>
          </div>
          <div class="track-shipment">
            <input
              class="form-control"
              type="text"
              placeholder="Enter your tracking number"
            />
            <Button content="Track" />
          </div>
        </div>
        <div class="read-more">
          <div class="text">Read More</div>
          <div class="icon"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "./misc/Button";
export default {
  name: "HeroSection",
  components: {
    Button
  }
};
</script>

<style lang="scss" scoped>
@import "../assets/styles/_colors.scss";
.hero-section {
  position: relative;
  .background {
    background: url("../assets/images/bg-hero.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    padding: 250px 0 200px;

    .content {
      color: #fff;
      .main-content {
        display: flex;
        align-items: center;
        .text {
          flex: 2;
          .main-text {
            text-transform: capitalize;
            font-size: 56px;
            font-weight: 600;
          }
          .sub-text {
            text-transform: capitalize;
            font-size: 18px;
            letter-spacing: 0.5px;
          }
        }
        .button {
          display: flex;
          align-items: center;
          justify-content: center;
          flex: 1;
          button {
            background: $theme-color;
            display: table;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            border: 0;
            outline: 0;
            color: #fff;
            padding: 21px 40px;
            font-weight: 550;
            border-radius: 5px;
            transition: 300ms all;
            box-shadow: 2px 2px 13px 3px rgba(255, 255, 255, 0.3);
            &:hover {
              box-shadow: 4px 10px 15px 10px rgba(255, 255, 255, 0.3);
            }
          }
        }
      }
      .track-shipment {
        padding: 0 200px;
        display: flex;
        align-items: center;
        margin-top: 60px;

        input {
          margin-right: 10px;
          padding: 20px 10px;
          border-radius: 3px;
        }
      }
    }

    .read-more {
      color: #fff;
      position: absolute;
      bottom: 50px;
      left: 50%;
      transform: translateX(-50%);
      font-weight: 20px;
      text-transform: uppercase;
      .icon {
        margin: 0 auto;
        margin-top: 15px;
        width: 20px;
        height: 20px;
        background: transparent;
        border-radius: 5px;
        border-right: 6px solid $theme-color;
        border-bottom: 6px solid $theme-color;
        transform: rotate(45deg);
        cursor: pointer;
      }
    }
  }
}

@media (max-width: 991px) {
  .hero-section {
    .background {
      padding: 200px 0 150px;
      .content {
        .main-content {
          .text {
            .main-text {
              font-size: 35px;
            }
            .sub-text {
              font-size: 16px;
            }
          }
          .button {
            button {
              padding: 15px 30px;
              font-size: 14px;
            }
          }
        }
        .track-shipment {
          padding: 0 100px;
        }
      }
    }
  }
}
@media (max-width: 767px) {
  .hero-section {
    .background {
      .content {
        .main-content {
          flex-direction: column;
          .button {
            margin-top: 30px;
          }
        }
        .track-shipment {
          padding: 0;
          input {
            padding: 15px 8px;
            font-size: 14px;
          }
        }
      }
    }
  }
}

@media (max-width: 991px) {
  .hero-section {
    .background {
      padding: 200px 0 150px;
      .content {
        .main-content {
          .text {
            .main-text {
              font-size: 28px;
            }
            .sub-text {
              font-size: 14px;
            }
          }
          .button {
            button {
              padding: 13px 26px;
              font-size: 13px;
            }
          }
        }
      }
      .read-more {
        bottom: 25px;
        .text {
          font-size: 14px;
        }
        .icon {
          margin-top: 10px;
          width: 15px;
          height: 15px;
          border-width: 4px;
        }
      }
    }
  }
}
</style>
