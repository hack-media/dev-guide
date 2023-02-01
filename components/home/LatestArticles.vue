<template>
  <section class="mt-7">
    <div>
      <h2 class="color-linear">Latest Articles</h2>
      <p>Discover the most outstanding articles in all topics</p>
    </div>

    <div class="row mt-5">
      <div
        v-for="article in latestArticles"
        :key="article.title"
        class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-3"
      >
        <div class="card-blog hover-up">
          <div class="card-image mb-3">
            <NuxtLink to="/">
              <img
                src="~/assets/images/news4.png"
                alt=""
              />
            </NuxtLink>
          </div>

          <div>
            <div class="row">
              <div class="col-12 text-end text-muted">
                <span>6 mins read</span>
              </div>
            </div>

            <NuxtLink to="/">
              <h5 class="mt-4">
                Self-observation is the first step of inner unfolding
              </h5>
            </NuxtLink>

            <div class="row align-items-center mt-4">
              <div class="col-7">
                <div class="box-author text-muted">
                  <img
                    src="~/assets/images/author.png"
                    alt=""
                  />
                  <div>
                    <h6>Joseph</h6>
                    <span>2 Feb 2023</span>
                  </div>
                </div>
              </div>

              <div class="col-5 text-end">
                <NuxtLink to="/">
                  <span>Read more</span>
                </NuxtLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

     <IncludesReadMore />
  </section>
</template>

<script setup lang="ts">
const latestArticles = [
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
  {
    title: 'Aenean Auctor Wisi Et Urna Aliquam Erat',
  },
];
</script>

<style scoped>
.card-blog {
  position: relative;
  padding: 1.2rem;
  width: 100%;
  border-radius: 0.5rem;
  margin-bottom: 1.8rem;
  background-color: #07575b5e;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
    rgba(0, 0, 0, 0.3) 0px 30px 60px -30px;
}

.card-blog .card-image img {
  border-radius: 0.5rem;
}

.box-author {
  display: flex;
  align-items: center;
}

.box-author img {
  display: inline-block;
  margin-right: 15px;
  height: 48px !important;
  width: 48px !important;
  border-radius: 0.5rem !important;
}

.box-author > div {
  width: 100%;
}

@media (max-width: 349.98px) {
  .box-author img {
    margin-right: 10px;
    height: 32px;
    width: 32px !important;
  }
}
</style>
