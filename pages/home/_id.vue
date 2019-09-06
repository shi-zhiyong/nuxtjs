<template>
  <div class="home-id-page">
    _id.vue
    {{ info }}
  </div>
</template>

<script>
  export default {
    asyncData(context) {
      console.log('asyncData', context);
      return {info: "hello world"}
    },
    fetch({ store, params }) {
      console.log('fetch', store);
      console.log('fetch', params);
    },
    beforeCreate() {
    },
    created() {
    },
    beforeMount() {
      console.log('beforeMount',window);
    },
    mounted() {
      console.log('mounted',window);
    }
  }
</script>

<style
  scoped>

</style>
