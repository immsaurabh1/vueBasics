<template lang="html">

  <nav class="navbar-component">
    <h1>
      <div class="navbar-flex ">
        <div>
       <span class="title" >
            <img src="https://static.shortlyst.com/assets/campaigns/Shopalyst_White_RobotoCondensed_1533899706853.png" class="img-logo">
        </span>
        </div>
          <div>svdwevwefw</div>

        </div>

    </h1>
  </nav>

</template>

<script lang="js">
  export default  {
    name: 'navbar-component',
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
.navbar-component {
  background-color: #006494;
  padding: 20px;
  position: fixed;
  width: 100%;
  top: 0;
  left:0;
  color:white;
}
.navbar-flex {
  display: flex;
  justify-content: space-between;
}
.img-logo{
  height:20px;
  width:auto;
}
</style>
