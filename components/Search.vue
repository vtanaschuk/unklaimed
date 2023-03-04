<template>
    <div class="search-component">
      <div class="container flex-grid">
        <div class="text w50">
          <div class="search-component-block">

          <div class="top-title">
            <span>
              Unclaimed property
            </span>
          </div>
          <div class="sub-title">
            <span class="first">Find out if you have some </span>
            <span class="second">Unclaimed Property</span>
          </div>
          <div class="paragraph">
            <p>Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.</p>
          </div>
          <div class="input-wrapper">
            <input type="text" placeholder="Name or Case Number" class="search-text">
            <select name="country" class="search-selector">
              <option value="">State</option>
              <option value="Ukraine">Ukraine</option>
              <option value="UK">UK</option>
              <option value="USA">USA</option>
            </select>
            <input type="submit" value="Search" class="search-btn">
          </div>
          <form class="search">
            <button class="header_search_btn"><img class="white" src="~/assets/img/search.png"></button>
            <input type="text" class="header_search_input" placeholder="Search claims"/>
          </form>


          </div>
        </div>
        <div class="img w50">
          <img src="~/assets/img/content_1_.png"  alt="logo"/>
        </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>

</style>