<template>
    <div>
      <ul class="d-inline-flex flex-column">
          <li v-for="numero in numeros" v-bind:key="numero" class="bg-light py-3 my-3 px-5 d-flex flex-column border border-success">
            {{numero.nombre}}
          <button class="btn btn-success btn-sm d-block mt-3" @click="numero.cantidad++">{{numero.cantidad}}</button>
          </li>
      </ul>
    </div>
</template>

<script>
export default {
  name: 'Fill',
  props:['numeros'],
  data(){
    return{
      array:[],
      numero:{
        nombre:'',
        cantidad:''
      }
    }
  },
}
</script>

