<script>
export default {
    props: {
        name: String, 
        salary: Number, 
        age: Number
    },
    data() {
        return {
        }
    }
}
</script>

<template>
<p class="user">{{ name }} 
<br>
{{ salary }} 
<br>
{{ age }}</p>
</template>