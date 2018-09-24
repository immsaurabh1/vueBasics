<template lang="html">

  <section class="base-multi-select-dropdown">
  {{label}}
  <ul v-for="item in menuOptions"> 
    <li v-if="isArrayNotObject" >
      {{item}}
    </li>
    <li v-if="!isArrayNotObject" >
      {{item.name}}
    </li>
  </ul>
  </section>

</template>

<script lang="js">
  export default  {
    name: 'base-multi-select-dropdown',
    props: [
      'selected','options', 'isArrayNotObject','label'
    ],
    mounted() {

    },
    data() {
      return {
        selected:this.selected,
        isArrayNotObject:this.isArrayNotObject,
        menuOptions:this.options,
        label: this.label
      }
    },
    methods: {

    },
    computed: {

    }
}
</script>

<style scoped lang="scss">
  .base-multi-select-dropdown {

  }
</style>
