
<template>
    <div class="">
        <button style="{{ background : color }}" class="px-2 py-1 text-white rounded-md font-bold"> {{ text }} </button>
    </div>
</template>

<script>
 export default {
    name : "Button",
    props : {
        text : String,
        color : String
    }
 }
</script>