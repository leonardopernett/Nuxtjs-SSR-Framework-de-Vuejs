<template>
  <h1>welcome to my first nuxt app</h1>
</template>

<script>
export default {
  head(){
    return{
      title:'home nuxt',
      meta:[
        {
          name:'description',
          content:'website about'
        }
      ],
      htmlAttrs:{
         lang:'en'
        }
    }
   }
  }
</script>