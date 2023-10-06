<template>
  <ion-app>
    <ion-router-outlet />
  </ion-app>
</template>

<script setup lang="ts">
import { IonApp, IonRouterOutlet } from '@ionic/vue';
import { createApp } from 'vue'; // Importa createApp de Vue para configurar la aplicación
import router from './router'; // Importa tu archivo de rutas

const app = createApp({});
app.use(router); // Usa el enrutador en tu aplicación Vue
app.mount('#app'); // Monta la aplicación en el elemento con el id "app"

</script>
