<template>
  <!--  元件的互動-->
     <div>
       <h2>學生姓名:{{ name }}</h2>
       <h2>學生年齡:{{ age }}</h2>
       <button @click="showName">點我提示學生姓名</button>
     </div>
  </template>
  
  <!--<style>-->
  <!--  /*css樣式*/-->
  <!--  .demo{-->
  <!--    background: skyblue;-->
  <!--  }-->
  <!--</style>-->
  
  
  <script>
    //元件互動的程式碼
    //export default school分別暴露
    export default {
      name: 'Student', //開發者工具最終呈現的名字為School
      data(){
        return {
          name:'panyue',
          age:21
        }
      },
      methods:{
        showName(){
          alert(this.name);
        }
      }
    };
  
    //統一暴露
    // export { school };
    // export default school //預設暴露
  </script>
  