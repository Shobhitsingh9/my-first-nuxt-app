<template>
<div>
   <input type="text" v-model="userId">
   <button @click="onLoaduser">Load user</button>
   <nuxt-child />
   </div>
   </template>

<script>
export default {
  data() {
    return {
      UserId: ''
    }
  },
  methods:{
     onLoaduser(){
    this.$router.push('/users/' + this.userId)
     }
  },
   layout:  'users',
   }
</script>
