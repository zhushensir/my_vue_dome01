<template>
  <div>
    <header class="site-header jumbotron">
      <div class="container">
        <div class="row">
          <div class="col-xs-12">
            <h1>请发表对vue的评论</h1>
          </div>
        </div>
      </div>
    </header>
    <div class="container">
    <!-- <Add :addComment="addComment"/> -->
    <List :comments="comments"/>
    </div>
  </div>  
</template> 

<script>
import Add from  './components/Add.vue'
import List from './components/List.vue'
export default {
  data(){ 
    return{
         comments:[ //数据在哪个组件，操作数据的行为（方法）就应该定义在哪个组件
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
  methods:{
    //添加评论
    addComment(comments){
      this.comments.unshift(comment)
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