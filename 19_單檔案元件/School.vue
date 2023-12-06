<template>
  <!--  元件的互動-->
     <div class="demo">
       <h2>學校名稱:{{ name }}</h2>
       <h2>學校地址:{{ address }}</h2>
       <button @click="showName">點我提示學校名</button>
     </div>
  </template>
  
  <style>
    /*css樣式*/
    .demo{
      background: skyblue;
    }
  </style>
  
  
  <script>
    //元件互動的程式碼
    //export default school分別暴露
    export default {
      name: 'School', //開發者工具最終呈現的名字為School
      data(){
        return {
          name:'武漢科技大學',
          address: '武漢'
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
  