<script setup>
// variable
const msg = 'Hello!'
const todos = [
 {item : "Learn Javascript"},
  {item : "Learn Vue Js"},
  {item: "Build something awesome"}
]

// functions
function log() {
  console.log(msg)
}
</script>

<template class="my-2" >
  <!-- <button >{{ msg }}</button> -->
  <div class="w-8/12 mx-auto">
    <ol>
      <li v-for="(todos,index) in todos" v-bind:key="todos.item" class="rounded bg-white my-1 px-4 py-1"> {{ index }} -  {{ todos.item}} </li>
    </ol>
  </div>
</template>

