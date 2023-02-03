<template>
  <section class="row mt-7">
    <div class="col-lg-12">
      <div>
        <h2 class="color-linear">Recent Posts</h2>
        <p>Don't miss the latest trends</p>
      </div>

      <div class="row mt-5">
        <div
          v-for="article in recentArticles"
          class="col-lg-6"
        >
          <div class="card-list-posts">
            <div class="card-image hover-up">
              <NuxtLink :to="`/blog/${article.title}/`">
                <img
                  src="~/assets/images/img7.jpg"
                  alt=""
                />
              </NuxtLink>
            </div>

            <div class="card-info">
              <NuxtLink :to="`/blog/${article.title}/`">
                <h5 class="mb-3">
                  How to Grow Your Business on Instagram in 2022
                </h5>
              </NuxtLink>

              <p>
                Gosh jaguar ostrich quail one excited dear hello and bound and
                the and bland moral misheard roadrunner flapped lynx far that
                and jeepers giggled far and far
              </p>

              <div class="row">
                <div class="col-12 date">
                  <span> 29 Jan 2023 </span>
                  <span class="time-read"> 3 mins read </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <IncludesReadMore />
    </div>
  </section>
</template>

<script setup lang="ts">
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
.card-list-posts {
  display: flex;
  width: 100%;
  margin-bottom: 4rem;
}

.card-list-posts .card-image {
  width: 270px;
  max-width: 170px;
  min-width: 170px;
  margin-right: 1rem;
}

.card-list-posts .card-image img {
  width: 100%;
  border-radius: 0.5rem;
}

.card-list-posts .card-info {
  width: 100%;
}

.card-list-posts .card-info p {
  color: #66768f;
  font-size: 0.9rem;
}

.card-list-posts .card-info .date {
  font-size: 0.8rem;
}

.card-list-posts .card-info .time-read {
  display: inline-block;
  padding: 0px 0px 0px 23px;
}

.card-list-posts .card-info a:hover h5 {
  color: #1cc2e7 !important;
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
</style>
