<template>
    <div>
        <ul>
          <li v-for="item in items" v-bind:key="item" v-bind:todo="item">{{item}}</li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'Fill',
  data (){
    return{
      items:['item 1', 'item 2', 'item 3']
    }
  }
}
</script>