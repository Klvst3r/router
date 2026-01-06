components: { Blog, }, components: { Users, },
<template>
  <div v-if="$route.params.userId">
    <div id="nav">
      <nav>
        <RouterLink :to="'/users/' + $route.params.userId"> Inicio </RouterLink>
        |

        <RouterLink :to="'/users/' + $route.params.userId + '/profile'">
          Perfil
        </RouterLink>
        |

        <RouterLink :to="'/users/' + $route.params.userId + '/courses'">
          Cursos
        </RouterLink>
      </nav>
    </div>

    <hr />

    <RouterView />
  </div>

  <div v-else>
    <h1>Users</h1>
    <p>Aquí podrás ver la lista completa de usuarios.</p>
  </div>
</template>

<script>
// Nota: No te hace falta importar Blog ni Users dentro de sí mismo,
// eso causaría una recursión infinita o errores de carga.
export default {
  name: 'UsersView',
}
</script>
<style scoped></style>
