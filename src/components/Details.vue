<template>
  <div v-if="error">
      <h1>{{error}}</h1>
  </div>
  <div v-if="post" class="post">
      <h3>{{post.title}} </h3>
      <p class="pre">{{post.body}}</p>
  </div>
  <div v-else><spinner/></div>
</template>

<script>
import getPost from '../composables/getPost'
import Spinner from '../components/Spinner.vue'
export default {
    name:'Details',
    components:{
        Spinner
    },
    props:[
        'id',
    ],
    setup(props){
       const {post, error, load} = getPost(props.id)
       load();     
        return {post, error}
    }
}
</script>

<style>

</style>