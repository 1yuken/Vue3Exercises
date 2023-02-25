<script>
export default {
    props: ['name', 'surn', 'age'],
    data() {
        return {
        }
    }
}
</script>

<template>
   <p class="user">{{ name }}</p>
   <p class="user">{{ surn }}</p>
   <p class="user">{{ age }}</p>
</template>