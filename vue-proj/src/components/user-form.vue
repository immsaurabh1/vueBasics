<template lang="html">

  <section class="user-form">
    <form>
      <h1>Create User</h1>
      <base-input :data="user.fName"></base-input>
      <base-input :data="user.lName"></base-input>
      <base-input :data="user.mailId"></base-input>
      <base-input :data="user.userName"></base-input>
      <!-- <base-multi-select-dropdown :selected="dropdown.selected" :options="dropdown.options" :isArrayNotObject="dropdown.isArrayNotObject" :label="dropdown.label" ></base-multi-select-dropdown> -->
      <div class="parent-org-drop"><div>
        <label>Select Parent Organisation</label></div>
        <div class="dropdown-section">
          <multiselect
            v-model="dropdown.selected"
            :options="dropdown.options">
          </multiselect>
    </div>
    </div>
    </form>
  </section>

</template>

<script lang="js">
import BaseInput from './base-input';
import Multiselect from 'vue-multiselect';
// import BaseMultiSelectDropdown from './base-multi-select-dropdown';
  export default  {
    name: 'user-form',
    components:{
      BaseInput,Multiselect
    },
    props: [],
    mounted() {

    },
    data() {
      return {
        user:{
          fName:['First Name','fchf'],
          lName:['Last Name','tg'],
          mailId:['E-mail Id',''],
          userName:['Enter UserName','']
        },
        dropdown:{
          selected:'',
          options:["asas","game","soap","mouse"]
          // isArrayNotObject:true,
          // label:"select a brand"
          
        }
      }
    },
    methods: {

    },
    computed: {

    }
}
</script>

<style scoped lang="scss">
.user-form {
}
.parent-org-drop{
  text-align:left;
  padding:10px;
  label{
    font-size:14px;
    color:#006494;
  }

}
.dropdown-section{
  width:240px;
}
</style>
<style src="../../node_modules/vue-multiselect/dist/vue-multiselect.min.css"></style>

