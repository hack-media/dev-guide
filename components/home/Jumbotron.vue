<template>
  <div class="banner banner-home2">
    <div class="text-center">
      <h6 class="color-gray-600">Welcome to devguide blog</h6>
      <h1 class="color-white">
        Being<span class="color-linear"> Unique</span> is better<br
          class="d-none d-lg-block"
        />than being
        <span class="color-linear">Erfect</span>
      </h1>
    </div>

    <div class="text-center mt-50">
      <ul class="list-tags-col-5 mb-50 text-center">
        <li
          v-for="frame in frameworks"
          :key="frame.name"
        >
          <div
            class="card-style-2 hover-up hover-neon animate__ animate__fadeInUp animated"
            style="visibility: visible"
          >
            <div class="card-image">
              <!-- <a href="blog-archive.html"
                ><img
                  src="assets/imgs/page/homepage1/tag1.png"
                  alt="Genz"
              /></a> -->
            </div>
            <div class="card-info">
              <a
                class="color-gray-500"
                href="blog-archive.html"
                >{{ frame.name }}</a
              >
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
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
  {
    name: 'Express',
  },
  {
    name: 'Go',
  },
  {
    name: 'Firebase',
  },
];
</script>

<style scoped>
.banner {
  padding-top: 50px;
}

.banner-home2 {
  padding-top: 80px;
}

.card-style-2 {
  border-width: 1px;
  border-style: solid;
  padding: 19px;
  position: relative;
  display: flex;
  border-radius: 16px;
  align-items: center;
  margin-bottom: 30px;
}

.card-style-2 .card-image {
  width: 32px;
  height: 32px;
  margin-right: 8px;
  min-width: 32px;
}

.card-style-2 .card-image img {
  width: 32px;
  height: 32px;
  border-radius: 50%;
}

.card-style-2 .card-info a:hover {
  color: #1CC2E7;
}

.list-tags-col-5 {
  display: flex;
  margin: 0px -10px;
  flex-wrap: wrap;
  justify-content: center;
}

.list-tags-col-5 li {
  flex: 0 0 auto;
  width: 20%;
  padding: 0px 10px;
  min-width: 150px;
  max-width: 180px;
}

.hover-neon {
  transition: all 0.25s cubic-bezier(0.02, 0.01, 0.47, 1);
  border: 1px solid #222f43;
  background-color: #131c31;
}

.hover-neon:hover {
  background: linear-gradient(#131c31, #131c31) padding-box,
    linear-gradient(to right, rgb(14, 165, 234), rgb(11, 209, 209)) border-box;
  border-radius: 16px;
  border: 1px solid transparent;
  box-shadow: rgba(11, 209, 209, 0.2) 0px 3px 20px;
  transform: translateY(-2px);
  transition: all 0.25s cubic-bezier(0.02, 0.01, 0.47, 1);
}
</style>
