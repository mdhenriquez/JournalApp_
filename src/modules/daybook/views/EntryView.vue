<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div>
      <span class="text-success fs-3 fw-bold">24</span>
      <span class="mx-1 fs-3">Abril</span>
      <span class="mx-2 fs-4 fw-light">2024, Miércoles</span>
    </div>
    <div>
      <button class="btn btn-danger">
        Borrar
        <i class="fa-solid fa-trash"></i>
      </button>
      <button class="btn btn-success">
        Subir Todo
        <i class="fa-solid fa-upload"></i>
      </button>
    </div>
  </div>
  <hr />
  <div class="d-flex flex-column px-3 h-75">
    <textarea placeholder="Qué sucedió hoy?"></textarea>
  </div>
  <Fab icon="fa-solid fa-pen" />

  <img
    src="https://i.ibb.co/f2pJN4J/shrek.jpg"
    alt="Shrek Windows"
    class="img-thumbnail"
  />
</template>

<script>
import { defineAsyncComponent } from 'vue';
export default {
  components: {
    Fab: defineAsyncComponent(() => import('../components/Fab.vue')),
  },
};
</script>

<style lang="scss" scoped>
textarea {
  font-size: 20px;
  border: none;
  height: 100%;

  &:focus {
    outline: none;
  }
}

img {
  width: 200px;
  position: fixed;
  bottom: 150px;
  right: 20px;
  box-shadow: 0px 5px 10px rgba($color: #000, $alpha: 0.2);
}
</style>
