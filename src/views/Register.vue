<template>
  <BasicLayouts>
    <div class="register">
      <h2>Registro de usuario</h2>
      <form class="ui form">
        <div class="field">
          <input type="text" placeholder="Nombre de usuario" />
        </div>
        <div class="field">
          <input type="text" placeholder="Correo eletronico" />
        </div>
        <div class="field">
          <input type="password" placeholder="Contraseña" />
        </div>

        <button type="submit" class="ui button fluid primary">
          Crear usuario
        </button>
      </form>

      <router-link to="/login">
        Iniciar sesión
      </router-link>
    </div>
  </BasicLayouts>
</template>

<script>
import BasicLayouts from '../layouts/BasicLayouts.vue';
export default {
  components: { BasicLayouts },
  name: 'Register',
};
</script>

<style lang="scss" scoped>
.register {
  text-align: center;
  h2 {
    margin: 50px 0 30px 0;
  }

  .ui.form {
    max-width: 300px !important;
    margin: 0 auto;
    margin-bottom: 10px;
    input.error {
      border-color: #faa;
      background-color: #ffeded;
    }
  }
}
</style>
