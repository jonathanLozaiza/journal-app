<template>
  <div
    class="entry-container mb-3 pointer p-2"
    @click="$router.push({ name: 'entry', params: { id: 10 } })"
  >
    <!--Titulo-->
    <div class="entry-title d-flex">
      <span class="text-success fs-5 fw-bold">15</span>
      <span class="mx-1 fs-5">Julio</span>
      <span class="mx-2 fs-5 fw-light">2021, jueves</span>
    </div>
    <div class="entry-description">
      Mollit mollit duis voluptate consectetur magna reprehenderit voluptate
      anim ut est amet quis. Proident eiusmod amet tempor laboris dolor et
      incididunt. Minim do exercitation labore tempor irure reprehenderit nulla
      sint esse quis aliquip proident. Eiusmod nisi non quis reprehenderit et ex
      sint. Ipsum qui laboris qui non nostrud sunt pariatur. Quis aliquip culpa
      laboris esse eu ad adipisicing anim id quis.
    </div>
  </div>
</template>

<script>
export default {
  name: "Entry",
};
</script>

<style lang="scss" scoped>
.entry-container {
  border-bottom: 1px solid #2c3e50;
  transition: 0.2s all ease-in;
  &:hover {
    background-color: lighten($color: grey, $amount: 45);
    transition: 0.2s all ease-in;
  }
  .entry-description {
    font-size: 11px;
  }
}
</style>
