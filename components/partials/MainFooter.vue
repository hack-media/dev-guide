<template>
  <footer class="footer mt-7">
    <div class="container">
      <div class="footer-1 bg-gray-850 border-gray-800">
        <div class="row">
          <div class="col-lg-4 mb-30">
            <a href="index.html">
              <!-- <img
                src="assets/imgs/template/logo.svg"
                alt=""
              /> -->
            </a>
            <p class="mb-20 mt-20 text-sm color-gray-500">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Perspiciatis ipsum ab nam accusantium. Corrupti, ab libero ad
              tempore quod dicta.
            </p>
            <h6 class="mb-5">Address</h6>
            <p class="text-sm color-gray-500">East Legon<br />Ghana, Accra</p>
          </div>

          <div class="col-lg-4 mb-30">
            <h6 class="text-lg mb-30">Categories</h6>
            <div class="row">
              <div class="col-6">
                <ul class="menu-footer">
                  <li
                    v-for="frame in frameworks"
                    :key="frame.name"
                  >
                    <a
                      class="color-gray-500"
                      href="blog-archive.html"
                    >
                      {{ frame.name }}
                    </a>
                  </li>
                </ul>
              </div>

              <div class="col-6">
                <ul class="menu-footer">
                  <li
                    v-for="frame in frameworks"
                    :key="frame.name"
                  >
                    <a
                      class="color-gray-500"
                      href="blog-archive.html"
                    >
                      {{ frame.name }}
                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </div>

          <div class="col-lg-4 mb-30">
            <h4 class="text-lg mb-30">Newsletter</h4>
            <p class="text-base color-gray-500">
              Sign up to be first to receive the latest stories inspiring us,
              case studies, and industry news.
            </p>
            <div class="form-newsletters mt-15">
              <form action="#">
                <div class="form-group">
                  <input
                    class="input-name border-gray-500"
                    type="text"
                    placeholder="Your name"
                  />
                </div>
                <div class="form-group">
                  <input
                    class="input-email border-gray-500"
                    type="email"
                    placeholder="Email address"
                  />
                </div>
                <div class="form-group mt-20">
                  <button class="btn btn-linear hover-up">
                    Subscribe
                    <i class="fi-rr-arrow-small-right"></i>
                  </button>
                </div>
              </form>
            </div>
          </div>
        </div>

        <div class="footer-bottom border-gray-800">
          <div class="row">
            <div class="col-lg-5 text-center text-lg-start">
              <p class="text-base">
                © 2023<a
                  class="copyright"
                  href="#"
                  target="_blank"
                >
                  sources
                </a>
              </p>
            </div>

            <div class="col-lg-7 text-center text-lg-end">
              <div class="box-socials">
                <div class="d-inline-block mr-30">
                  <a
                    class="icon-socials icon-twitter color-gray-500"
                    href="https://twitter.com"
                  >
                    Twitter
                  </a>
                </div>
                <div class="d-inline-block mr-30">
                  <a
                    class="icon-socials icon-linked color-gray-500"
                    href="https://www.linkedin.com"
                  >
                    LinkedIn
                  </a>
                </div>
                <div class="d-inline-block">
                  <a
                    class="icon-socials icon-insta color-gray-500"
                    href="https://www.instagram.com"
                  >
                    Instagram
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
const frameworks = [
  {
    name: 'Vue',
  },
  {
    name: 'Nuxt',
  },
  {
    name: 'React',
  },
  {
    name: 'Next',
  },
  {
    name: 'Django',
  },
  {
    name: 'Electron',
  },
];
</script>

<style scoped>
.footer {
  position: relative;
  z-index: 2;
}

.copyright {
  color: #1cc2e7;
}
.copyright:hover {
  color: #0ea5ea;
}
.footer-1 {
  margin: 50px 0px 24px 0px;
  padding: 89px 128px 50px 128px;
  border-radius: 48px;
  border-width: 1px;
  border-style: solid;
}
.footer .icon-socials {
  display: inline-block;
  padding-left: 28px;
  height: 32px;
  width: auto;
  transition-duration: 0.2s;
}
.footer .icon-socials:hover {
  transform: translateY(-3px);
  transition-duration: 0.2s;
  color: rgb(14, 165, 234) !important;
}
.footer .icon-socials.icon-twitter {
  background: url(../imgs/template/icons/tw.svg) no-repeat 0px 0px;
  transition-duration: 0.2s;
}
.footer .icon-socials.icon-twitter:hover {
  background: url(../imgs/template/icons/tw-hover.svg) no-repeat 0px 0px;
  transition-duration: 0.2s;
}
.footer .icon-socials.icon-insta {
  background: url(../imgs/template/icons/insta.svg) no-repeat 0px 0px;
  transition-duration: 0.2s;
}
.footer .icon-socials.icon-insta:hover {
  background: url(../imgs/template/icons/insta-hover.svg) no-repeat 0px 0px;
  transition-duration: 0.2s;
}
.footer .icon-socials.icon-linked {
  background: url(../imgs/template/icons/linked.svg) no-repeat 0px 0px;
  transition-duration: 0.2s;
}
.footer .icon-socials.icon-linked:hover {
  background: url(../imgs/template/icons/linked-hover.svg) no-repeat 0px 0px;
  transition-duration: 0.2s;
}
.footer .menu-footer {
  display: inline-block;
}
.footer .menu-footer li {
  list-style: none;
  margin-bottom: 12px;
}
.footer .menu-footer li a {
  font-size: 16px;
  line-height: 24px;
  text-decoration: none;
  display: block;
  padding: 0px 0px 0px 0px;
  transition-duration: 0.2s;
}
.footer .menu-footer li a:hover {
  color: #0ea5ea !important;
  transition-duration: 0.2s;
  padding-left: 3px;
}

.footer .footer-bottom {
  border-top-width: 1px;
  border-top-style: solid;
  padding: 50px 0px 0px 0px;
  font-size: 14px;
}
.footer .footer-bottom a {
  text-decoration: none;
}

.box-socials {
  display: inline-block;
  margin-top: 0px;
}
.box-socials a {
  display: inline-block;
  height: 50px;
  width: 50px;
  border-radius: 50%;
  margin-right: 10px;
  transition: all 0.2s;
}
.box-socials a span {
  display: inline-block;
  height: 50px;
  width: 50px;
  border-radius: 50%;
}
.box-socials a span.fb {
  background-image: url(../imgs/page/homepage3/fb.svg);
  background-repeat: no-repeat;
  background-position: center;
}
.box-socials a span.inst {
  background-image: url(../imgs/page/homepage3/inst.svg);
  background-repeat: no-repeat;
  background-position: center;
}
.box-socials a span.snap {
  background-image: url(../imgs/page/homepage3/snap.svg);
  background-repeat: no-repeat;
  background-position: center;
}
.box-socials a span.tw {
  background-image: url(../imgs/page/homepage3/tw.svg);
  background-repeat: no-repeat;
  background-position: center;
}
.box-socials a:hover {
  background: linear-gradient(
      90deg,
      rgb(14, 165, 234),
      rgb(11, 209, 209) 51%,
      rgb(14, 165, 234)
    )
    var(--x, 0) / 200%;
  transition: all 0.2s;
}

.footer .box-socials a {
  border-radius: 0px;
}

@media (max-width: 767.98px) {
  .footer-1 {
    padding: 89px 20px 50px 20px;
  }
}

@media (max-width: 991.98px) {
  .footer-bottom .box-socials {
    margin-top: 15px;
  }
}

@media (max-width: 1199.98px) {
  .footer-1 {
    padding: 89px 30px 50px 30px;
  }
}

.input-name,
.input-email {
  border: 0px;
  padding: 12px 12px 12px 20px;
  border-bottom-width: 1px;
  border-bottom-style: solid;
  background-color: transparent;
  width: 100%;
  color: #ffffff;
  background: url(../imgs/template/icons/user.svg) no-repeat left center;
}

.form-group {
  margin-bottom: 24px;
}

.text-base {
  font-family: 'Noto Sans', sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
}
</style>
