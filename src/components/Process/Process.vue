<template>
  <div class="process-section">
    <div class="process-section-inner">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <LeftContent />
          </div>
          <div class="col-md-6">
            <RightContent />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LeftContent from "./LeftContent";
import RightContent from "./RightContent";
export default {
  name: "Process",
  components: {
    LeftContent,
    RightContent
  }
};
</script>

<style lang="scss" scoped>
.process-section {
  padding: 50px 0;
}
</style>
