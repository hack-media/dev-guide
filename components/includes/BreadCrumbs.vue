<template>
  <section class="custom-breadcrumb">
    <ul>
      <li>
        <NuxtLink :to="{ name: 'index' }"> Home </NuxtLink>
      </li>
      <li><NuxtLink to="/">Blog</NuxtLink></li>
      <li>
        <span>Digital Design That Will Help You Start Your Business</span>
      </li>
    </ul>
  </section>
</template>

<style scoped>
.custom-breadcrumb {
  display: inline-block;
  margin: 2rem 0;
}

.custom-breadcrumb ul {
  display: flex;
  flex-wrap: wrap;
}

.custom-breadcrumb li:after {
  font: var(--fa-font-solid);
  content: '\f0da';
  padding: 0 0.5rem;
}

.custom-breadcrumb li:last-child::after {
  content: '';
}
</style>
