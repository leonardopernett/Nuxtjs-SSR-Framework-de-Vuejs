<template>
    <div>
        <h3>Posts</h3>
        <Post 
        v-for="post of posts"
        :key="post.id"
        :title="post.title" 
        :id="post.id" />
    </div>
</template>



<script>
import axios from 'axios'
import Post from '../../components/Post'
export default {
    components:{
         Post
        },
    data(){
        return {
           posts:[]
        }
    },
    async created(){
       const res = await axios.get('https://jsonplaceholder.typicode.com/posts');
       this.posts = res.data
    } 
}
</script>

<style  scoped>
 h3 {
    color:red
    } 
</style>