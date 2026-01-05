components: { Blog, }, components: { Users, },
<template>
  <div v-if="$route.params.userId">
    <h1>User</h1>
    <p>Aqui podrás ver el detalle de un usuario.</p>
  </div>
  <div v-else>
    <h1>Users</h1>
    <p>Aqui podrás ver la lista de usuarios.</p>
  </div>
  <div id="nav">
    <nav>
      <RouterLink to="/">Perfil</RouterLink>
      <RouterLink to="/about">Cursos</RouterLink>
    </nav>
  </div>
</template>

<script>
import Order from '@/views/Order.vue'
import Users from '@/views/Users.vue'
import Blog from '@/views/Blog.vue'

export default {}
</script>

<style scoped></style>
