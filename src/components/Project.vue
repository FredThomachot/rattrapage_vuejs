<template>  

 
      <div class="col-md-4">
          <h2>{{title.name}}</h2>
          <h3 v-if = "title.isActive === true">actif</h3>  
          <h3 v-else class="nonActif">non actif</h3>

          <input type="checkbox" id="checkbox" v-model="checked" v-if = "title.isActive === true"><label for="checkbox">actif</label>
          
          

          <h6 >Date de création: {{title.creation}}</h6>  

      </div>
    

</template>

<script>
export default {
  name: 'Project',
  props: ["title"],
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>

.col-md-4 {
  border-color: #42b983;
  border-style: solid;
  border-width: 1px;
  text-align:end;
  margin: 5px;
}
.nonActif {
  color:lightgrey;

}


</style>