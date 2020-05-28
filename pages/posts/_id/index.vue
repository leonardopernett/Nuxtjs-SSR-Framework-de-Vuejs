<template>
   <div>
        <h1>details posts</h1>
         <p>{{post.title}}</p>
         <p>{{post.body}}</p>
   </div>
</template>


<script>
import axios from 'axios';
export default {
    data(){
        return {
          post:{}
        }
    },
    async created(){
        const id =  this.$route.params.id
        const res = await axios.get('https://jsonplaceholder.typicode.com/posts/'+id)
        this.post= res.data 
    }
}
</script>