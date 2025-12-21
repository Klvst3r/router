<template>
    <div class="post">
        <h1>Vista de un post de un determinado usuario</h1>
        <p>Hola desde el post: {{ $route.params.post }} del usuario: {{ $route.params.user }} </p>
    </div>
</template>

<script>
export default {
    mounted() {
        console.log(this.$route.params);
    }
}
</script>

<style scoped>
.post {
    padding: 20px;
}
</style>