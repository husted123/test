<template>
  <nav
    ref="navbar"
    class="navbar"
    role="navigation"
    aria-label="Main navigation"
  >
    <div>
      <!-- Logo -->
      <div class="wedio-logo-wrapper">
        <img
          src="../assets/images/logo-wedio-white.svg"
          alt="Wedio logo"
          class="lazyload wedio-logo"
        />
      </div>

      <!-- Main links -->
      <div class="main-links">
        <router-link
          to="/"
          :class="activeSort === 'home' ? 'link-active' : ''"
          @click="activeSort = 'home'"
          >Home</router-link
        >
        <router-link
          to="/about"
          :class="activeSort === 'about' ? 'link-active' : ''"
          @click="activeSort = 'about'"
          >About</router-link
        >
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    const activeSort = "home";
    return { activeSort };
  }
};
</script>

<style lang="scss" scoped>
@import "../assets/styles/variables.scss";
@import "../assets/styles/buttons.scss";

nav {
  height: 80px;
  padding: 0px 24px;
  background-color: $black;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  margin-bottom: 80px;
}

.wedio-logo-wrapper {
  min-width: 168px;
  margin-top: 16px;
  margin-bottom: 4px;
  .wedio-logo {
    height: 14px;
  }
}
link {
  color: $grey;
}
.main-links {
  a {
    padding: 0px;
    padding-bottom: 1px;
    margin: 8px 12px;
    color: $white;
    text-decoration: none;
  }

  .link-active {
    border-bottom: 1px solid $green;
  }
}
</style>
