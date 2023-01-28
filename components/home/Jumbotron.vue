<template>
  <div class="banner">
    <div class="text-center">
      <h1>
        <span class="color-linear">Unlocking</span> the Latest
        <br class="d-none d-lg-block" />Tech
        <span class="color-linear">Trends...</span>
      </h1>
    </div>

    <div class="mt-5">
      <ul class="list-tags">
        <li
          v-for="frame in frameworks"
          :key="frame.name"
        >
          <NuxtLink :to="{ name: 'index' }">
            {{ frame.name }}
          </NuxtLink>
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
  padding-top: 5rem;
}

.list-tags {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  text-align: center;
  gap: 0.8rem;
}

.list-tags li {
  flex: 0 0 auto;
  width: 20%;
  min-width: 150px;
  max-width: 180px;
  padding: 1.3rem;
  margin-bottom: 30px;
  border-radius: 0.5rem;
  transition: all 0.25s cubic-bezier(0.02, 0.01, 0.47, 1);
  border: 1px solid transparent;
  background-color: var(--ocean);
  font-weight: 600;
}

.list-tags li:hover {
  background: linear-gradient(var(--secondary), var(--secondary)) padding-box,
    linear-gradient(to right, #0ea5ea, #0bd1d1) border-box;
  box-shadow: #0bd1d133 0px 3px 20px;
  transform: translateY(-2px);
  transition: all 0.25s cubic-bezier(0.02, 0.01, 0.47, 1);
  cursor: pointer;
}

.list-tags li:hover a {
  color: inherit;
}
</style>
