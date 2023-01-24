<template>
  <main class="main">
    <div class="cover-home1">
      <div class="container">
        <div class="row">
          <div class="col-xl-1"></div>
          <div class="col-xl-10 col-lg-12">
            <HomeJumbotron />
            <HomeLatestArticles />
            <HomeRecentArticles />
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'HomePage',
};
</script>

<style scoped>
.cover-home1 {
  position: relative;
}
.cover-home1 .container {
  position: relative;
  z-index: 2;
}
.cover-home1::after {
  height: 800px;
  width: 500px;
  content: "";
  z-index: 1;
  background: url(../imgs/template/shadow-1.svg) no-repeat right top;
  position: absolute;
  left: 0px;
  top: 0px;
}
.cover-home1::before {
  height: 1500px;
  width: 500px;
  content: "";
  z-index: 1;
  background: url(../imgs/template/shadow-3.svg) no-repeat right bottom;
  position: absolute;
  right: 0px;
  top: 700px;
}

@media (max-width: 575.98px) {
  .cover-home1::before,
  .cover-home1::after {
    display: none;
  }
}
</style>
