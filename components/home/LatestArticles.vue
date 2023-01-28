<template>
  <div class="mt-70">
    <h2
      class="color-linear mb-10 wow animate__ animate__fadeInUp animated"
      style="visibility: visible; animation-name: fadeInUp"
    >
      Featured Articles
    </h2>
    <p
      class="text-lg color-gray-500 wow animate__ animate__fadeInUp animated"
      style="visibility: visible; animation-name: fadeInUp"
    >
      Discover the most outstanding articles in all topics
    </p>

    <div class="row mt-70">
      <div
        v-for="article in latestArticles"
        :key="article.title"
        class="col-lg-4"
      >
        <div
          class="card-style hover-up mb-30 wow animate__ animate__fadeIn animated"
          data-wow-delay=".0s"
          style="visibility: visible"
        >
          <div class="card-image">
            <a
              class="post-type"
              href="blog-archive.html"
            ></a
            ><a
              class="link-post"
              href="single-sidebar.html"
              ><img
                src="~/assets/images/news1.png"
                alt="Genz"
              />
              <div class="card-info card-bg-2">
                <div class="info-bottom mb-15">
                  <h4 class="mb-15">
                    Aenean Auctor Wisi Et Urna Aliquam Erat
                  </h4>
                  <div class="box-author">
                    <img
                      src="~/assets/images/news1.png"
                      alt="Genz"
                    />
                    <div class="author-info">
                      <h6 class="mr-15 color-gray-700">Thomson</h6>
                      <span class="color-gray-700 text-sm">25 April 2022</span>
                    </div>
                  </div>
                </div>
              </div></a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
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
];
</script>

<style scoped>
.card-style {
  position: relative;
  width: 100%;
}

.card-style:hover h6 {
  color: #1cc2e7 !important;
}

.card-style:hover .card-image img {
  transform: scale(1.1);
}

.card-style .card-image {
  border-radius: 8px;
  overflow: hidden;
  position: relative;
}

.card-style .card-image img {
  width: 100%;
  border-radius: 8px;
}

.card-style .card-image .link-post:hover h4 {
  color: #1cc2e7 !important;
}

.card-style .card-image .card-info {
  position: absolute;
  bottom: 0px;
  height: 100%;
  width: 100%;
  border-radius: 8px;
  background: url(../imgs/page/homepage1/bg-trans.png) repeat-x left bottom;
}

.card-style .card-image .card-info.card-bg-2 {
  background: url(../imgs/page/homepage3/bg-trans.png) repeat-x left bottom;
}

.card-style .card-image .card-info .info-bottom {
  position: absolute;
  bottom: 0px;
  left: 0px;
  padding: 15px;
}

.card-style .card-image .card-info .box-author img {
  width: 32px !important;
  height: 32px !important;
  border-radius: 50%;
}

.card-style .card-image .card-info .box-author .author-info {
  display: flex;
  align-items: center;
}

.card-style .card-image .card-info .box-author .author-info h6 {
  line-height: 20px !important;
}

.post-type {
  background: url(../imgs/template/icons/post-type.svg) no-repeat center;
  height: 42px;
  width: 42px;
  position: absolute;
  top: 15px;
  right: 15px;
}

.post-type.post-audio {
  background: url(../imgs/template/icons/post-audio.svg) no-repeat center;
}

.post-type.post-image {
  background: url(../imgs/template/icons/post-image.svg) no-repeat center;
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
  border-radius: 50% !important;
}

.box-author .author-info {
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
