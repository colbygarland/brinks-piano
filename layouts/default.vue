<template>
  <div>
      <PageHeader />
      <Nuxt />
      <footer class="bg-gray-900 text-white py-3 px-3">
          <div class="container mx-auto text-center">
              <p><small>&copy;2020 Brink's Piano Works. <br class="md:hidden" />All rights reserved. <br class="md:hidden" /> Website by <a class="font-bold" href="https://colbygarland.ca" target="_blank">Colby Garland</a></small></p>
          </div>
      </footer>
  </div>
</template>

<script>
import PageHeader from "~/components/Header";
import Content from "~/components/Content";

export default {
    components: {
        'PageHeader': PageHeader,
        'Content': Content,
    },
}
</script>
