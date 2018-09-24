<template lang="html">

  <section class="base-input">
    <label class="label">{{inputData[0]}}</label>
    <input class="custom-input" type="text" for="text" v-model="inputData[1]">
  </section>

</template>

<script lang="js">
  export default  {
    name: 'base-input',
    props: ['data'],
    mounted() {

    },
    data() {
      return {
       inputData: this.data
      }
    },
    methods: {

    },
    computed: {

  }}
</script>

<style scoped lang="scss">
  .base-input {
    width: 100%;
    text-align: left;
    padding: 10px;
  }
  .label{
    font-size:14px;
    color: #006494;
    display:block;
  }
  .custom-input{
    height:35px;
    width:240px;
    display:block;
  }
</style>
