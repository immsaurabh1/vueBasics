<template lang="html">

  <section class="body-component">
    <user-form></user-form>
  </section>

</template>

<script lang="js">
import UserForm from './user-form'
  export default  {
    name: 'body-component',
    components: { UserForm },
    props: [],
    mounted() {

    },
    data() {
      return {

      }
    },
    methods: {

    },
    computed: {

    }
}
</script>

<style scoped lang="scss">
  .body-component {
    padding-top: 30px;
    margin-right: 20px;
    margin-left: 20px;
  }
</style>
