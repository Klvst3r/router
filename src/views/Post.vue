<template>
    <div class="post">
        <h1>Título del post</h1>
        <p>Hola desde el post: {{ $route.params.post }}</p>
    </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const title = ref('')
const content = ref('')

onMounted(() => {
    // Fetch post data
})
</script>

<style scoped>
.post {
    padding: 20px;
}
</style>