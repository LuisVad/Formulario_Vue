<template>
  <div>
    <router-view />
  </div>
</template>

<script>
import Vue from 'vue';
import VueRouter from 'vue-router';
import Formulario from './components/Formulario.vue';

Vue.use(VueRouter);

const routes = [
  { path: '/', component: Formulario },
  { path: '/exito', component: Exito }, // Define un componente para la página de éxito
];

const router = new VueRouter({
  routes,
});

export default {
  name: 'App',
  router,
};
</script>
