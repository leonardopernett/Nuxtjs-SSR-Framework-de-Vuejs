<template>
   <div>
     <Navigation />
      <div class="content">
        <nuxt />
     </div>
   </div>
</template>




<script>
import Navigation from '../components/navigation'
export default {
  components:{
    Navigation
  }
}
</script>

<style>
  *{
     box-sizing: border-box;  
  }
  body {
    background: #2d3436;
    color:#fff
  }
  .content {
    padding:2rem;
  }
</style>