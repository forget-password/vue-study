<template>
  <div class="about" v-bind:title="data">
    <h1 v-on:click="handle">This is an about page {{ data }} --</h1>
  </div>
</template>
<script>
export default {
  data: () => ({
    data: 22,
  }),
  methods: {
    handle(e) {
      console.log(e, "=====", 22);
    },
  },
};
</script>
<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
