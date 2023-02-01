<template>
  <header class="header sticky-bar">
    <div class="container">
      <div class="main-header">
        <div class="header-logo">
          <NuxtLink
            class="d-flex"
            :to="{ name: 'index' }"
          >
            DevGuide
          </NuxtLink>
        </div>

        <div class="header-nav">
          <nav class="nav-main-menu d-none d-xl-block">
            <ul class="main-menu">
              <li>
                <a
                  class="color-gray-500"
                  href="page-contact.html"
                >
                  Home
                </a>
              </li>
              <li>
                <a
                  class="color-gray-500"
                  href="page-contact.html"
                >
                  Articles
                </a>
              </li>
              <li class="has-children">
                <a
                  class="color-gray-500"
                  href="page-about.html"
                  >About Me</a
                >
                <ul class="sub-menu">
                  <li>
                    <a
                      class="color-gray-500"
                      href="page-portfolio.html"
                      >My Portfolio</a
                    >
                  </li>
                </ul>
              </li>
            </ul>
          </nav>

          <div class="burger-icon burger-icon-white">
            <span class="burger-icon-top"></span
            ><span class="burger-icon-mid"></span
            ><span class="burger-icon-bottom"></span>
          </div>
        </div>

        <div class="header-right text-end">
          <a
            class="btn btn-search"
            href="#"
          ></a>
          <!-- <div class="form-search p-20">
            <form action="#">
              <input
                class="form-control"
                type="text"
                placeholder="Search"
              />
              <input
                class="btn-search-"
                type="submit"
                value=""
              />
            </form>
          </div> -->
          <!-- <a
            class="btn btn-linear d-none d-sm-inline-block hover-up hover-shadow"
            href="page-login.html"
          >
            Subscribe
          </a> -->
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.header {
  float: left;
  width: 100%;
  position: relative;
  /* background: var(--ocean) */
}

.header .main-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
  width: 100%;
  /* padding: 5px 0px; */
}

.header .main-header .header-logo {
  max-width: 150px;
  width: 100%;
}

.header .main-header .header-logo a {
  display: block;
  min-height: 37px;
  color: var(--primary);
  font-size: 1.2rem;
  font-weight: 600;
}

.header .main-header .header-nav {
  display: inline-block;
  width: 65%;
  text-align: center;
}

.header .main-header .header-right {
  max-width: 225px;
  width: 100%;
}
.header .main-header .header-right .block-signin {
  text-align: right;
}
.header .nav-main-menu {
  width: auto;
  padding: 0px;
  float: none;
}
.header .burger-icon {
  display: none;
}
.header .main-menu {
  display: inline-block;
  padding-top: 3px;
}
.header .main-menu li {
  float: left;
  position: relative;
  text-align: left;
}
.header .main-menu li.has-children > a::after {
  content: '\f151';
  font-family: uicons-regular-rounded !important;
  font-style: normal;
  font-weight: normal !important;
  font-variant: normal;
  text-transform: none;
  line-height: 1 !important;
  font-size: 14px;
  opacity: 1;
  margin-left: 0px;
  position: relative;
  top: 2px;
}
.header .main-menu li.hr {
  padding: 0px 22px;
}
.header .main-menu li.hr span {
  background-color: #d8e6fb;
  height: 1px;
  width: 100%;
  display: block;
  margin: 5px 0;
}
.header .main-menu li a {
  font-family: 'Noto Sans', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 16px;
  display: block;
  padding: 13px 17px;
  text-decoration: none;
  position: relative;
}
.header .main-menu li a:hover,
.header .main-menu li a.active {
  color: #1cc2e7;
}
.header .main-menu li a:hover i,
.header .main-menu li a.active i {
  opacity: 1;
  transition: 0.2s;
}
.header .main-menu li a i {
  font-size: 12px;
  margin-right: 8px;
  opacity: 0.38;
  transition: 0.2s;
}
.header .main-menu li ul {
  opacity: 0;
  visibility: hidden;
  transition-duration: 0.2s;
  position: absolute;
  top: calc(100% + 9px);
  left: 0px;
  z-index: 999999;
  min-width: 180px;
  border-radius: 0 0 4px 4px;
  padding: 8px 0px 8px 0;
  background: #131c31;
  /* Gray/800 [night] */
  border: 1px solid #222f43;
  box-shadow: 0px 23.1405px 69.4215px rgba(0, 0, 0, 0.12);
  border-radius: 8px;
}
.header .main-menu li ul li {
  width: 100%;
}
.header .main-menu li ul li a {
  font-size: 14px;
  color: #94a9c9;
  font-size: 13px;
  line-height: 16px;
  position: relative;
  padding: 10px 22px 10px 38px;
  background: url(../imgs/template/icons/icon-menu.svg) no-repeat left 20px
    center;
  transition: 0.2s;
}
.header .main-menu li ul li a:hover {
  transition: 0.2s;
  background: url(../imgs/template/icons/icon-menu-hover.svg) no-repeat left
    20px center;
}
.header .main-menu li ul li a.closer {
  padding: 8px 22px 8px 22px;
}
.header .main-menu li ul li ul {
  top: 0px;
  left: 100%;
}
.header .main-menu li:hover > ul {
  opacity: 1;
  visibility: visible;
}
.header .main-menu li:hover > ul li {
  width: 100%;
}
.header .text-link-bd-btom {
  font-family: 'Noto Sans', sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 150%;
  color: #0f172a;
  display: inline-block;
  position: relative;
  padding-left: 13px;
}
.header .text-link-bd-btom:hover {
  color: #0f172a;
}
.header .text-link-bd-btom::before {
  content: '';
  background: #0f172a;
  width: 6px;
  height: 6px;
  border-radius: 50%;
  position: absolute;
  left: 0;
  top: 50%;
  margin-top: -3px;
  animation: shadow-pulse 1s infinite;
}
.header .block-signin .btn-shadow {
  box-shadow: 0px 47px 65px rgba(21, 28, 38, 0.1);
}

.burger-icon {
  position: absolute;
  width: 24px;
  height: 20px;
  cursor: pointer;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1);
  top: 15px;
  right: 0px;
  z-index: 99999999;
}

.burger-icon > span {
  display: block;
  position: absolute;
  left: 0;
  width: 100%;
  height: 2px;
}

.burger-icon > span.burger-icon-top {
  top: 2px;
}

.burger-icon > span.burger-icon-bottom {
  bottom: 2px;
}

.burger-icon > span.burger-icon-mid {
  top: 9px;
}

.burger-icon > span::before,
.burger-icon > span::after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
  background-color: #333;
}

.burger-icon.burger-icon-white > span::before,
.burger-icon.burger-icon-white > span::after {
  background-color: #94a9c9;
}

@media (max-width: 499.98px) {
  .form-search {
    right: 0;
  }
}

@media (max-width: 575.98px) {
  .header .main-header .header-right {
    padding-right: 25px;
  }

  .header .container {
    max-width: 100%;
  }

  .header {
    padding: 0px 0;
  }
}

@media (max-width: 767.98px) {
  .burger-icon {
    top: 17px;
  }
}

@media (max-width: 1199.98px) {
  .header .main-header .header-nav {
    width: 0%;
  }

  .header .burger-icon {
    display: block;
  }

  .header .main-header .header-right {
    max-width: 285px;
    padding-right: 35px;
  }

  .burger-icon {
    display: inline-block;
  }
}

.form-search {
  position: absolute;
  /* top: 100%; */
  right: 98px;
  width: 100%;
  max-width: 350px;
  z-index: 999;
  background-color: #0b1222;
  padding: 5px 5px;
  /* display: none; */
  border-radius: 8px;
  border: 1px solid #222f43;
}

.form-search .form-control {
  height: 46px;
  background-color: #0f172a;
  border-color: #222f43;
  font-size: 14px;
  line-height: 1;
  padding: 10px 15px 10px 20px;
}

.form-search .btn-search-2 {
  position: absolute;
  top: 22px;
  right: 28px;
  width: 40px;
  height: 40px;
  background: white;
  border: 0px;
}

.form-control::-webkit-date-and-time-value {
  color: #66768f;
  font-size: 14px;
  line-height: 18px;
}

.btn.btn-search {
  height: 42px;
  width: 42px;
  /* background: url(../imgs/template/icons/icon-search.svg) no-repeat center; */
}
</style>
