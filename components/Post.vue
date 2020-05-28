<template>
    
    <nuxt-link :to="'/posts/' + id">
       <div class="post">
        <p>{{id}} - {{title}}</p>
    </div>
    </nuxt-link>
</template>


<script>
export default {
    name:'Post',
    props:['id','title']
}
</script>

<style>
   .post {
      padding:1rem;
      border: 1px solid #ccc;
      margin:1rem 0 ;
    }
    .post:hover{
      cursor :pointer;
       background: #2d3436;
       color:#fff;
       border:1px solid blue
    }
    a{
        text-decoration: none;
        color:#fff
    }
</style>