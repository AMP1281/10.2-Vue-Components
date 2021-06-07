<template>
    <div class="test text-center py-5 px-5 border border-success">
        <h3>Component Pare</h3>
        <Fill :numeros="items"></Fill>
    </div>
</template>

<script>

import Fill from './Fill.vue'

export default {
  name: 'Pare',
  components: {
    Fill
  },
    data (){
    return{
      items:[
        {nombre:'item 1', cantidad:0},
        {nombre:'item 2', cantidad:0},
        {nombre:'item 3', cantidad:0}
      ]
    }
  }
}
</script>

<style>

.test{background: rgb(199, 199, 199) !important;}

</style>