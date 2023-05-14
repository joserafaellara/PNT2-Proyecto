<script>
  import Cabecera from './components/Cabecera.vue'
  import Pie from './components/Pie.vue'
  import Proyecto from './components/Proyecto.vue'
 

  export default
  (await import('vue')).defineComponent({
    components: {Cabecera,Pie,Proyecto},
    data(){
      return{
        nEmpresa : "Grupo: Puntos Plus"
      }
    }
  })
  
</script>

<template>
   <div>
      <Cabecera/>
      <Proyecto/>
      <Pie :empresa="nEmpresa" />
   </div>
</template>

<style scoped>

</style>
