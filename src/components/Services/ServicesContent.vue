<template>
  <div class="row">
    <div class="col-md-4">
      <div class="service">
        <div class="img-block">
          <img src="../../assets/images/job-board.png" alt="service-img" />
        </div>
        <div class="text-block">
          <div class="heading">Job Board</div>
          <div class="text">
            Best job opportunities! Matching the requirements between employe...
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <div class="service">
        <div class="img-block">
          <img
            src="../../assets/images/buy-sell-and-lease.png"
            alt="service-img"
          />
        </div>
        <div class="text-block">
          <div class="heading">Buy Sell & Lease</div>
          <div class="text">
            Buy, sell, or lease a truck or other equipment fast. Post your pr...
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <div class="service">
        <div class="img-block">
          <img src="../../assets/images/marketplace.png" alt="service-img" />
        </div>
        <div class="text-block">
          <div class="heading">Marketplace</div>
          <div class="text">
            Buy or Sell New or Used Parts and Tires effortlessly! List your p...
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <div class="service">
        <div class="img-block">
          <img
            src="../../assets/images/finance-and-factoring.png"
            alt="service-img"
          />
        </div>
        <div class="text-block">
          <div class="heading">FINANCE / FACTORING</div>
          <div class="text">
            Find premium loan offers to purchase the equipment you need. No c...
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <div class="service">
        <div class="img-block">
          <img
            src="../../assets/images/question-ansswer.png"
            alt="service-img"
          />
        </div>
        <div class="text-block">
          <div class="heading">QUESTION / ANSWER</div>
          <div class="text">
            Have a question and need someone to guide you? Post your question...
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <div class="service">
        <div class="img-block">
          <img src="../../assets/images/insurance.png" alt="service-img" />
        </div>
        <div class="text-block">
          <div class="heading">INSURANCE</div>
          <div class="text">
            Find a professional insurance agent that meets all your needs. Of...
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ServicesContent"
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/_colors.scss";
.row {
  margin-bottom: 50px;
  .service {
    padding: 20px;
    padding-bottom: 30px;
    text-align: center;
    transition: 500ms all;
    cursor: pointer;
    &:hover {
      box-shadow: 2px 2px 30px 5px rgba(0, 0, 0, 0.2);
    }
    .text-block {
      .heading {
        margin: 15px 0 10px;
        font-size: 20px;
        font-weight: 600;
        text-transform: uppercase;
      }
      .text {
        color: $light-gray-text;
      }
    }
  }
}
</style>
