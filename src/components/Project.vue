<template>  
    <div  id="datasName">
        <h1>{{title.name}}</h1>
        <h2>Projet actif : {{title.isActive}}</h2>    
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