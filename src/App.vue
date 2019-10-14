<template>
  <div id="app">
    <div>
      <header class="site-header jumbotron">
        <div class="container">
          <div class="row">
            <div class="col-xs-12">
              <h1>请发表对Vue的评论</h1>
            </div>
          </div>
        </div>
      </header>
      <div class="container">
        <Add/>
        <List :comments='comments'/>
      </div>
    </div>
  </div>  
</template>

<script>  
  import Add from './components/Add.vue'
  import List from './components/List.vue'
  
  export default{
    data(){
      return{
        comments:[
        {name:'bob',content:'1234'},
        {name:'nancy',content:'129'},
        {name:'tom',content:'0989'},
      ]
      }
    },
    components:{
      Add,
      List
    }
  }
</script>

<style>

</style>
