<template>
  <div>
    <h1>Öğrenciler</h1>
     <div v-for="student in students" :key="student.id">
       <router-link  :to="{path:`/students/${student.id}`}">{{ student.name }}</router-link>
       <!-- <router-link  :to="{name:'studentsInfo',params:{id:student.id}}">{{ student.name }}</router-link> -->

    </div>         
  </div>
</template>

<script>
export default {
  data(){
    return {
        students:[
               {id:1,name:'Ahmet Mustafa',not:55},
               {id:2,name:'Metin Tanışman',not:55},
               {id:3,name:'Okan Doruk',not:65},
               {id:3,name:'Emirhan Altunel',not:85}, 
               {id:3,name:'Uğurcan Hallaçoğlu',not:75},


        ]
    }
  }
}
</script>

<style>

</style>