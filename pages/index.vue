<template>
  <header>
    <nav class="container flex-grid">
      <div class="menu"><a @click="menuOpen()"><img src="~/assets/img/Menu.png" alt=""></a></div>
      <div class="">
        <NuxtLink to="/" class="img-link">
          <img src="~/assets/img/logo.png"  alt="logo"/>

        </NuxtLink>
      </div>
      <div class="header-links">
        <!--      <NuxtLink class="header-link">About</NuxtLink>-->
        <!--      <NuxtLink to="/faq" class="header-link">FAQ</NuxtLink>-->
        <!--      <NuxtLink to="/contact" class="header-link">Contact</NuxtLink>-->
        <a @click="scrollTo('about-span')" class="header-link">About</a>
        <a @click="scrollTo('how-it-work')" class="header-link">How it works</a>
        <a @click="scrollTo('faq-span')" class="header-link">FAQ</a>
        <a @click="scrollTo('contact')" class="header-link">Contact</a>

      </div>
      <div class="push">
        <form class="header_search">
          <button class="header_search_btn"><img class="white" src="~/assets/img/search.png"><img class="black" src="~/assets/img/img.png"></button>
          <input type="text" class="header_search_input" placeholder="Search claims"/>
        </form>
        <NuxtLink class="sign-up-btn" to="/sign_in"><img src="~/assets/img/login.png">
          <span class="sign-up-btn-span">Sign in / Sign up</span>
        </NuxtLink>
        <NuxtLink class="basket-btn" to="/basket">
          <img src="~/assets/img/Buy.png"  alt="logo"/>
        </NuxtLink>
      </div>
    </nav>
  </header>
  <search />
  <span ref="about-span"></span>
  <about />
  <span ref="how-it-work"></span>
  <howItWork />
  <advantages />
  <span ref="faq-span"></span>
  <faq />
  <span ref="contact"></span>
  <contact />
  <Footer />
</template>

<script>
export default {
  methods: {
    scrollTo(name) {
      this.$refs[name]?.scrollIntoView({ behavior: 'smooth' })
    },
    menuOpen() {
      document.querySelector('.header-links').classList.toggle('show');
    }
  },
  watch: {
    '$route.query'(query) {
      if (query.id) {
        this.scrollTo(query.id)
      }
    },
  },

}
</script>

<style scoped>
h2{
  margin: 10px;
  font-size: 36px;
}
p{
  margin: 5px;
  font-size: 20px;
}
</style>