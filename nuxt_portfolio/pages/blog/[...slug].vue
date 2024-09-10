<script setup lang="ts">
const { slug } = useRoute().params;
</script>

<template>
  <div class="container">
    <ContentDoc :path="`/blog/${slug}`"">
      <template v-slot="{doc}">
      
      <section
        data-bs-version="5.1"
        class="article12 cid-u8fMpe3KhD"
        id="article12-2q"
      >
        <div class="container">
          <div class="row justify-content-center">
            <div class="col-md-12 col-lg-10">
              <ContentRenderer :value="doc"></ContentRenderer>
            </div>
          </div>
        </div>
      </section>
      </template>
      <template #not-found>
      <h1>Not found</h1>
      </template>
    </ContentDoc>
  </div>
</template>


