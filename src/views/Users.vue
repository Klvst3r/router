components: { Users, },
<template>
  <div v-if="$route.params.userId">
    <h1>User</h1>
    <p>Aqui podrás ver el detalle de un usuario.</p>
  </div>
  <div v-else>
    <h1>Users</h1>
    <p>Aqui podrás ver la lista de usuarios.</p>
  </div>
</template>

<script>
import Order from '@/views/Order.vue'
import Users from '@/views/Users.vue'

export default {}
</script>

<style scoped></style>
