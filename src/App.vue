<script setup>
  import users from '../users.json'
</script>

<template>
  <div class="container" >
       <div class="row">
          <div class="col-md-12">
             <div class="table-responsive">
                <table class="table">
                   <thead class="thead-dark">
                      <tr>
                         <th scope="col">Nombre</th>
                         <br>
                         <th scope="col">Genero</th>
                         <br>
                         <th scope="col">Pais</th>
                         <br>
                         <th scope="col">Imagen</th>
                         <!--Holaaa-->
                      </tr>
                   </thead>
                   <tbody>
                      <tr v-for="users in users" v-bind:key="users.gender">
                         <td>{{users.name.title}},{{users.name.first}},{{users.name.last}}</td>
                         <br>
                         <td>{{users.gender}}</td>
                         <br>
                         <td>{{users.location.country}}</td>
                      </tr>
                   </tbody>
                </table>
  
             </div>
          </div>
       </div>
    </div>
    
</template>

<style scoped>

</style>
