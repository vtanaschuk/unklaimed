<template>
  <div class="faq" ref="element2">
    <div class="container">
      <div class="top-title">
        <span class="top">FAQ</span>
      </div>
      <div class="sub-title">
        <span>Quick Assists</span>
      </div>
    </div>
    <div class="container">
      <div class="toggle">
        <span @click="showMessage = !showMessage" class="faq-title">Question1</span>
        <p class="faq-content"  v-show="showMessage">Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.</p>
      </div>
      <div class="toggle">
        <span @click="showMessage1 = !showMessage1" class="faq-title">Question1</span>
        <p class="faq-content"  v-show="showMessage1">Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.</p>
      </div>
      <div class="toggle">
        <span @click="showMessage2 = !showMessage2" class="faq-title">Question1</span>
        <p class="faq-content"  v-show="showMessage2">Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.</p>
      </div>
      <div class="toggle">
        <span @click="showMessage3 = !showMessage3" class="faq-title">Question1</span>
        <p class="faq-content"  v-show="showMessage3">Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showMessage: false,
      showMessage1: false,
      showMessage2: false,
      showMessage3: false

    };
  }
};

</script>

<style scoped>

</style>