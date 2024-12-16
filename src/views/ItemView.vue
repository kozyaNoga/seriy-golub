<template>
    <div>Товар {{ $route.params.id }}</div>
</template>
<script>
    export default{
        data() {
            return {
                user_data: null,
            }
        }
    }
</script>