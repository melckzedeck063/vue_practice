<template>
   <div class="bg-slate-100 h-full pb-4">
    <div class="bg-slate-700 p-2">
        <HeaderComponent  />
    </div>
    <div class="w-10/12 mx-auto my-4">
        <h1 class="text-blue-600 text-center font-medium text-4xl" > {{ msg}} </h1>
        <p class="text-slate-800 text-sm" > Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorum accusantium dicta rem architecto, cumque eos expedita beatae rerum natus laborum obcaecati tempore quas, tenetur ea, cum nobis eligendi atque sunt? </p>
    </div>
   </div>
</template>

<script>
import HeaderComponent from './HeaderComponent.vue';

 export default {
    name: "DemoPage",
    props: {
        msg: String
    },
    components: { HeaderComponent }
}
</script>