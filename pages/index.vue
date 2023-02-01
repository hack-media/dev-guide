<template>
  <main>
    <div class="container">
      <div class="row">
        <div class="col-12">
          <HomeJumbotron />
          <HomeLatestArticles />
          <HomeRecentArticles />
        </div>
      </div>
    </div>
  </main>
</template>

<script setup lang="ts">
useHead({
  title: 'Dev Guide - Unlocking the latest tech trend',
  meta: [{ name: 'description', content: 'Unlocking the latest tech trend' }],
});
</script>
