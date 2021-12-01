<template>
    <!-- Button -->
<button id="myBtn" @click="onClick()">Anders' Button</button>
</template>
<script>
export default {
    name: "Button",
    methods:{
    onClick() {
    var modal = document.getElementById("myModal");
      modal.style.display = "block";
    },
}}
</script>