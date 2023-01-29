<template>
  <section class="row mt-5">
    <div class="col-lg-12">
      <div>
        <h2 class="color-linear">Recent Posts</h2>
        <p>Don't miss the latest trends</p>
      </div>

      <div class="box-list-posts mt-5">
        <div class="row">
          <div
            v-for="article in recentArticles"
            class="col-lg-6"
          >
            <div
              class="card-list-posts card-list-posts-small wow animate__ animate__fadeIn animated"
              style="visibility: visible; animation-name: fadeIn"
            >
              <div class="card-image hover-up">
                <a href="single-sidebar.html"
                  ><img
                    src="~/assets/images/img7.jpg"
                    alt="Genz"
                /></a>
              </div>
              <div class="card-info">
                <a href="single-sidebar.html">
                  <h5 class="mb-15">
                    How to Grow Your Business on Instagram in 2022
                  </h5></a
                >
                <p class="color-gray-500">
                  Gosh jaguar ostrich quail one excited dear hello and bound and
                  the and bland moral misheard roadrunner flapped lynx far that
                  and jeepers giggled far and far
                </p>
                <div class="row mt-20">
                  <div class="col-12">
                    <span class="calendar-icon color-gray-700 text-sm mr-25"
                      >29 May 2022</span
                    ><span class="color-gray-700 text-sm timeread"
                      >3 mins read</span
                    >
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="text-start mb-80">
        <a
          class="btn btn-linear btn-load-more wow animate__ animate__zoomIn animated"
          style="visibility: visible; animation-name: zoomIn"
          >Show More Posts<i class="fi-rr-arrow-small-right"></i
        ></a>
      </div>
    </div>
  </section>
</template>

<script setup>
const recentArticles = [
  {
    title: 'How to Grow Your Business on Instagram in 2022',
  },
  {
    title: 'How to Grow Your Business on Instagram in 2022',
  },
  {
    title: 'How to Grow Your Business on Instagram in 2022',
  },
  {
    title: 'How to Grow Your Business on Instagram in 2022',
  },
  {
    title: 'How to Grow Your Business on Instagram in 2022',
  },
  {
    title: 'How to Grow Your Business on Instagram in 2022',
  },
];
</script>

<style scoped>
.calendar-icon {
  background: url(../imgs/template/icons/calendar.svg) no-repeat left center;
  display: inline-block;
  padding-left: 23px;
  padding-top: 2px;
}

.card-list-posts {
  display: flex;
  width: 100%;
  margin-bottom: 60px;
}

.card-list-posts .card-image {
  width: 270px;
  min-width: 270px;
  margin-right: 20px;
}

.card-list-posts .card-image img {
  width: 100%;
  border-radius: 16px;
}

.card-list-posts .card-info {
  width: 100%;
}

.card-list-posts .card-info a:hover h3,
.card-list-posts .card-info a:hover h4,
.card-list-posts .card-info a:hover h5 {
  color: #1cc2e7 !important;
}

.card-list-posts .card-info .col-7 a:hover {
  color: #0ea5ea !important;
}

.card-list-posts.card-list-posts-small .card-image {
  max-width: 170px;
  min-width: 170px;
}

@media (max-width: 767.98px) {
  .card-list-posts .card-image {
    width: 160px;
    min-width: 160px;
  }
}

@media (max-width: 499.98px) {
  .card-list-posts {
    flex-wrap: wrap;
  }

  .card-list-posts .card-image {
    width: 100%;
    min-width: 100%;
    margin-bottom: 30px;
  }
}

.timeread {
  background: url(../imgs/page/homepage1/clock.svg) no-repeat left center;
  display: inline-block;
  padding: 0px 0px 0px 23px;
}

.btn.btn-load-more {
  border-radius: 80px;
  padding: 18px 30px;
}

.btn.btn-load-more i {
  display: inline-block;
  vertical-align: middle;
}
</style>
