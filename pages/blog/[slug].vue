<template>
  <article>
    <IncludesBreadCrumbs />

    <div class="row mb-5">
      <div class="col-lg-8 m-auto text-center">
        <h2 class="color-linear">
          Digital Design That Will Help You Start Your Business
        </h2>
      </div>
    </div>

    <div class="row">
      <div class="col-lg-8 m-auto">
        <div class="row mb-4">
          <div class="col-md-6">
            <div class="author">
              <img
                src="~/assets/images/author.png"
                alt="author"
              />
              <div class="author-info">
                <h6>William Randolph</h6>
                <span class="me-3">25 April 2022</span>
                <span>3 mins to read</span>
              </div>
            </div>
          </div>

          <div class="col-md-6 text-start text-md-end">
            <div class="d-inline-block">
              <h6 class="d-inline-block me-3">Share</h6>
              <a
                class="icon-media"
                href="/"
              >
                <i class="fa-brands fa-facebook"></i>
              </a>
              <a
                class="icon-media"
                href="/"
              >
                <i class="fa-brands fa-twitter"></i>
              </a>
              <a
                class="icon-media"
                href="/"
              >
                <i class="fa-brands fa-discord"></i>
              </a>
            </div>
          </div>
        </div>

        <div class="content-detail">
          <p>
            The fancy moon going in little artist painting. Thirty days of
            lavender in the dreamy light inside. Other perfect oh plants, for
            and again. I’ve honey feeling. Caring dreamland projects noteworthy
            than minimal, their it oh pretty feeling may. Include pink be.
          </p>

          <div class="my-4">
            <img
              class="blog-image"
              src="~/assets/images/img.jpg"
              alt=""
            />
          </div>

          <p>
            Tortor placerat bibendum consequat sapien, facilisi facilisi
            pellentesque morbi. Id conse ctetur ut vitae a massa a. Lacus ut
            bibendum sollicitudin fusce sociis mi. Dictum volutpat praesent
            ornare accumsan elit venenatis. Congue sodales nunc quis ultricies
            odio porta. Egestas mauris placerat leo phasellu s ut sit.
          </p>

          <h3 class="color-linear">Use your headings</h3>
          <p>
            Thirty there &amp; time wear across days, make inside on these you.
            Can young a really, roses blog small of song their dreamy life
            pretty? Because really duo living to noteworthy bloom bell.
            Transform clean daydreaming cute twenty process rooms cool. White
            white dreamy dramatically place everything although. Place out
            apartment afternoon whimsical kinder, little romantic joy we flowers
            handmade. Thirty she a studio of she whimsical projects, afternoon
            effect going an floated maybe.
          </p>

          <h3 class="color-linear">Use your headings</h3>
          <p>
            Thirty there &amp; time wear across days, make inside on these you.
            Can young a really, roses blog small of song their dreamy life
            pretty? Because really duo living to noteworthy bloom bell.
            Transform clean daydreaming cute twenty process rooms cool. White
            white dreamy dramatically place everything although. Place out
            apartment afternoon whimsical kinder, little romantic joy we flowers
            handmade. Thirty she a studio of she whimsical projects, afternoon
            effect going an floated maybe.
          </p>
        </div>
      </div>
    </div>
  </article>
</template>

<script setup lang="ts">
const route = useRoute();
const routeParam = ref(route.params.slug);

useHead({
  title: 'Blog Details - Unlocking the latest tech trend',
  meta: [{ name: 'description', content: 'Unlocking the latest tech trend' }],
});
</script>

<style scoped>
.author {
  display: flex;
  align-items: center;
}

.author img {
  display: inline-block;
  margin-right: 1rem;
  height: 48px !important;
  width: 48px !important;
  border-radius: 50% !important;
}

.author .author-info {
  width: 100%;
}

.icon-media {
  margin: 0 0.5rem;
}

.content-detail {
  padding-bottom: 2rem;
  border-bottom-width: 1px;
  border-bottom-style: solid;
  margin-bottom: 2rem;
}

.content-detail .blog-image {
  border-radius: 16px;
  width: 100%;
}

h3 {
  margin: 2rem 0;
  font-size: 2rem;
  font-weight: 600;
}
</style>
