<style scoped>
  .select {
    border: none;
    border-bottom: 1px solid #ced4da;
    width: calc(100% - 2.5rem);
    width: 100%;
    padding-left: 0px;
    /* margin-left: 2.5rem; */
  }
</style>
<template>
  <!-- Card -->
  <mdb-card style="max-width: 500px;margin-left: auto;margin-right: auto;padding:40px">
    <mdb-card-body>
      <form>
        <p class="h4 text-center py-4">Sign up</p>
        <div class="grey-text text-left">
          <mdb-input placeholder="Your name" group type="text" validate error="wrong" success="right"/>
          <mdb-input placeholder="Your age" group type="number" validate error="wrong" success="right"/>
          <div class="md-form">
            <!-- <i style="font-size: 1.75em;position: absolute; top: 0.25em; left: 0" class="fas prefix fa-exclamation-triangle" /> -->
            <select class="browser-default custom-select select">
              <option value="1">Your gender</option>
              <option value="1">Male</option>
              <option value="2">Female</option>
            </select>
          </div>  
        </div>
        <div class="text-center py-4 mt-3">
          <mdb-btn color="cyan" type="submit">Register</mdb-btn>
        </div>
      </form>
    </mdb-card-body>
  </mdb-card>
  <!-- Card -->
</template>
<script>
  import { mdbInput, mdbBtn, mdbCard, mdbCardBody } from 'mdbvue';
  export default {
    name: 'Join',
    components: {
      mdbInput,
      mdbBtn,
      mdbCard,
      mdbCardBody
    },
    data() {
      return {
        genderOptions: [
          { text: 'Male', value: 'male' },
          { text: 'Female', value: 'female' }
        ]
      };
    }
  }
</script>
