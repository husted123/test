<template>
  <footer>
    <div class="container">
      <div>
        <ul class="footer-list">
          <li>
            <a class="link" href="#" rel="noopener">Rent Gear</a>
          </li>
          <li>
            <a class="link" href="#" rel="noopener">Subscription</a>
          </li>
          <li>
            <a class="link" href="#" rel="noopener">Lender</a>
          </li>
          <li>
            <a class="link" href="#" rel="noopener">How it works</a>
          </li>
          <li>
            <a class="link" href="#" rel="noopener">Blog</a>
          </li>
          <li>
            <a class="link" href="#" rel="noopener">Jobs</a>
          </li>
        </ul>
      </div>
      <hr id="separator" />
      <div class="soc-media-container">
        <a
          class="soc-media "
          href="https://www.facebook.com/WedioGlobal"
          target="_blank"
          rel="noopener"
        >
          <img
            src="../assets/images/fb-black.svg"
            alt="Icon of the facebook"
            class="soc-media-circle"
          />
        </a>
        <a
          class="soc-media "
          href="https://www.instagram.com/wedio_community"
          target="_blank"
          rel="noopener"
        >
          <img
            src="../assets/images/instagram-black.svg"
            alt="Icon of the instagram"
            class="soc-media-circle"
          />
        </a>
        <a
          class="soc-media "
          href="https://www.linkedin.com/company/wedio/"
          target="_blank"
          rel="noopener"
        >
          <img
            src="../assets/images/linkedin-black.svg"
            alt="Icon of the linkedin"
            class="soc-media-circle"
          />
        </a>
      </div>

      <div class="copyright">
        <p>© 2018-{{ new Date().getFullYear() }}</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "../assets/styles/variables.scss";

footer {
  background-color: $black;
  padding: 20px 40px 40px 40px;
}

a,
link {
  color: $grey;
}

li {
  padding: 20px 15px 0px 15px !important;
  a {
    text-decoration: none;
  }
  display: inline-block;
}

#separator {
  background-color: #000;
  height: 1px;
  margin-top: 40px;
  margin-bottom: 40px;
  border: 0;
}

.copyright {
  text-align: center;
  color: $white;
  margin-top: 28px;
}

.soc-media-container {
  margin-bottom: 20px !important;
  .soc-media {
    padding: 0px 6px;
    &:hover {
      filter: invert(100%);
    }

    .soc-media-circle {
      height: 34px;
    }
  }
}

.footer-list {
  display: inline-block;
  margin: 0 auto;
  padding: 0;
  list-style: none;
  text-decoration: none;
  position: relative;
}
</style>
