<template>
  <div id="app">
    <div class="container-fluid">

       <section-news></section-news>
    </div>
  </div>

</template>

<script>
import SectionNews from "./components/SectionNews.vue";

export default {
  name: "App",
  components: {
    SectionNews,
  }
}
</script>

