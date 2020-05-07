<template>
  <div>
    <header class="site-header jumbotron">
      <div class="container">
        <div class="row">
          <div class="col-xs-12">
            <h1>请发表对React的评论</h1>
          </div>
        </div>
      </div>
    </header>
    <div class="container">
    <Add/>
    <List :comments="comments"/>
    </div>
  </div>  
</template>

<script>
import Add from  './components/Add.vue';
import List from './components/List.vue';
export default {
  data(){
    return{
      comments:[
        {
          name:'Bob',
          content:'vue 初步看懂'
        },
        {
          name:'CAT',
          content:'Vue so Easy'
        },
        {
          name:'BZ',
          content:'JUST so so'
        }
      ]
    }
  },
  components:{ 
    Add,
    List
  }
};
</script>

<style>
</style>