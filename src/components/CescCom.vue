<template>
<div>
  <div>
    <pre>{{JSON.stringify(formValues, null, 1)}}</pre>
  </div>
  <div>
    <form>
      <div id="user-input-css">
        <label for="css">Css</label>
        <input type="checkbox" id="css" value="css" v-model="formValues.skillSet">
      </div>  
      <div id="user-input-js">
        <label for="js">js</label>
        <input type="checkbox" id="js" value="js" v-model="formValues.skillSet">
        
      </div>  
      <div id="user-input-html">
        <label for="html">html</label>
        <input type="checkbox" id="hmtl" value="html" v-model="formValues.skillSet">        
      </div>  
      <div id="radius">
        <div>
         <label for="no exp">no exp</label>
        <input type="radio" id="no exp" value="no exp" v-model="formValues.yearsExp">     
      </div>
      <div>
         <label for="enough exp">enough exp</label>
        <input type="radio" id="enough exp" value="enough exp" v-model="formValues.yearsExp">     
      </div>
      <div>
         <label for="too many">too many</label>
        <input type="radio" id="too many" value="too many" v-model="formValues.yearsExp">     
      </div>
      </div>
      <div>
        <label>Hola Cesc</label>
        <div>
          <label id="only" for="only"></label>
          <input type="checkbox" id="only" value="only" v-model="formValues.test">
        </div>
      </div>

      

    </form>
  </div>
</div>
</template>

<script>
export default {
  data() {
    return {
      formValues: {
        skillSet: [],
        yearsExp: "",
        test: ""
      }
    }
  }
}
</script>


<style>

</style>
