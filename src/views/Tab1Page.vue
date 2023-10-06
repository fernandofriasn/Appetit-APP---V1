<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Appetit</ion-title>
      </ion-toolbar>
    </ion-header>


    <ion-card color="dark">
    <ion-card-header>
      <ion-card-title >Menu</ion-card-title>
    </ion-card-header>

    <!-- <ion-card-content>
      Best Yuca Mash on City. Come and Join Us
    </ion-card-content> -->
  </ion-card>

    <ion-title>Rayli's Food Truck</ion-title>
    <ion-list>
    <ion-item>
      <ion-toggle color="success">Yuca/Huevo</ion-toggle>
    </ion-item>
    <ion-item>
      <ion-toggle color="success">Salchichas Fritas</ion-toggle>
    </ion-item>
    <ion-item>
      <ion-toggle color="success">Jugo Natural</ion-toggle>
    </ion-item>
  </ion-list>

  <ion-title>Felix's Food Truck</ion-title>
    <ion-list>
    <ion-item>
      <ion-toggle color="success">Hot Dog</ion-toggle>
    </ion-item>
    <ion-item>
      <ion-toggle color="success">Sandwich de Pierna</ion-toggle>
    </ion-item>
    <ion-item>
      <ion-toggle color="success">Coca Cola</ion-toggle>
    </ion-item>
  </ion-list>

  <ion-title>Haneury's Food Truck</ion-title>
    <ion-list>
    <ion-item>
      <ion-toggle color="success">Yaroa</ion-toggle>
    </ion-item>
    <ion-item>
      <ion-toggle color="success">Salchipapa</ion-toggle>
    </ion-item>
    <ion-item>
      <ion-toggle color="success">Refresco</ion-toggle>
    </ion-item>
  </ion-list>

  <!-- <ion-button expand="full" color="success">Order</ion-button> -->
  

  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';




 

</script>

<style>

span{
  text-align: right;
}

</style>