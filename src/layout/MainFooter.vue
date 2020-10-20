<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="https://www.instagram.com/thanh_so_khanh/">
              Hey Guys!
            </a>
          </li>
          <li>
            <a href="https://www.instagram.com/thanh_so_khanh/">
              About Us
            </a>
          </li>
          <li>
            <a href="https://www.instagram.com/thanh_so_khanh/">
              Blog
            </a>
          </li>
          <li>
            <a href="https://www.instagram.com/thanh_so_khanh/">
              Licenses
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, made with <md-icon>favorite</md-icon> by
        <a href="https://www.facebook.com/ThanhTranDung1405" target="_blank">Thành Kaido</a>
        for a better web.
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
