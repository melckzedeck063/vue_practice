/* eslint-disable */
<script setup>
const users = [
    {fname : "melckzedeck", lname : "james", email : "melckzedeck063@gmail.com", phone : "255744219981"},
    {fname : "ezekiel", lname: "michael", email : "ezekiel_michael@gmail.com", phone : "255743216789"},
    {fname : "rachel", lname:"jeremieh", email:"jeremiehrachel@gmail.com", phone : "255786901706"}
]
const msg  = "Hello";
// functions
function log() {
  console.log(msg)
}
</script>


<template>
    <div class="w-9/12 mx-auto my-4">
        <div class="">
            <div>{{ msg }}</div>
            <table>
                  <thead>
            <tr class="bg-slate-700">
                <th class="py-1.5 text-lg font-medium text-white px-4">S/NO</th>
                <th class="py-1.5 text-lg font-medium text-white px-4">Firstname</th>
                <th class="py-1.5 text-lg font-medium text-white px-4">Lastname</th>
                <th class="py-1.5 text-lg font-medium text-white px-4">Email</th>
                <th class="py-1.5 text-lg font-medium text-white px-4">Telephone</th>
                <th class="py-1.5 text-lg font-medium text-white px-4">Actions</th>
            </tr>
                  </thead>
                  <tbody>
                    
                        <tr v-for="(users, index) in users" :key="users.email" >
                            <td class="py-1.5 px-2 text-sm font-light text-slate-700 capitalize"> {{ index }} </td>
                            <td class="py-1.5 px-2 text-sm font-light text-slate-700 capitalize"> {{ users.fname }} </td>
                            <td class="py-1.5 px-2 text-sm font-light text-slate-700 capitalize"> {{ users.lname }} </td>
                            <td class="py-1.5 px-2 text-sm font-light text-slate-700">{{ users.email }}</td>
                            <td class="py-1.5 px-2 text-sm font-light text-slate-700">{{ users.phone }}</td>
                            <td class="py-1.5 px-2 text-sm font-light text-slate-700"> <ButtonComponent text="Edit" color="blue" /> </td>
                        </tr>
                    <!-- </div> -->
                  </tbody>
            </table>
            
        </div>
    </div>
</template>


<script>
  import ButtonComponent from './ButtonComponent.vue';
   export default {
    name : "TableHeader",
    components : {
       ButtonComponent 
    }
   }
</script>