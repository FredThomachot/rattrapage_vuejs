<template>  

 
      <div class="col-md-4">
          <h2>Projet : {{projet.name}}</h2>
          <h6>{{projet.description}}</h6>
        
          <!-- <h3 v-if = "projet.isActive === true">actif</h3>  
          <h3 v-else class="nonActif">non actif</h3>

          <input type="checkbox" id="checkbox" v-model="checked" v-on:click = "projet.isActive = !projet.isActive"><label for="checkbox">Changer état</label>
          
          <h6 >Date de création: {{projet.creation}}</h6>   -->

      </div>
    

</template>

<script>
export default {
  name: 'Project',
  props: ["projet"],
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>

.col-md-4 {
  background-color: aliceblue;
  border-color: #42b983;
  border-style: solid;
  border-width: 3px;
  text-align:justify;
  margin: 5px;
}
.nonActif {
  color:lightgrey;

}
h6 {
  font-size: 14px;
}


</style>