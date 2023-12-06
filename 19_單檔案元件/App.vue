<template>
  <div>
    <School></School>
    <Student></Student>
  </div>
</template>

<script>
import School from './School';
import Student from "./Student";

export default {
 name: "App",
 //彙總所有的元件
 components:{
   Student,
   School
 }
}
</script>

