<template>
  <div id="app"> 
    <Body/>
    <div class="container-card"> 
     <div class="card"  v-for="post of posts" :key="post.id">
       <Card :title="post.title" :body="post.body"/> 
     </div>
    </div>
  </div>
</template> 
<script>

 

import Post from './services/posts' 
import Card from './components/card' 
import Body from './components/body'  

export default {
  name: 'App',
  components: {
    Card,
    Body 
  }, 
  data(){
      return {
          posts:[]
      }
  },
  mounted(){
      Post.listar().then(response => {
          this.posts = response.data;
          console.log(this.posts);
      })
  }
}

</script>
 
<style>
body{
    font-family: sans-serif;
    color:white; 
    width: 100%;
    overflow-x: hidden; 
} 
 
 
*{
    margin:0;
    padding:0;
    box-sizing: border-box;
    
    
}
.container-card{
  display: flex; 
  flex-flow: row wrap;
  justify-content: center;
  width: 100%;
  padding-top: 20px;
}
</style>

 