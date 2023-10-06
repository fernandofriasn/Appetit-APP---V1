<template>
  <ion-card>
    <ion-card-header>
      <ion-card-title>Appetit </ion-card-title>
      <ion-card-subtitle>Your Fav Place to eat</ion-card-subtitle>
    </ion-card-header>

    <ion-card-content> Welcome to the Login Page </ion-card-content>
  </ion-card>

  <ion-input 
    label="Username:"
    label-placement="fixed"
    fill="solid"
    placeholder="Enter the username "
    color="danger"
  ></ion-input>

  <br />

  <ion-input
    label="Password:"
    type="password"
    label-placement="fixed"
    fill="outline"
    placeholder="Enter your password"
    color="danger"
  ></ion-input>

  <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
  <ion-button  expand="full" color="success">Login</ion-button>

</template>

<script lang="ts">
import {
  IonCard,
  IonCardContent,
  IonCardHeader,
  IonCardSubtitle,
  IonCardTitle,
  IonInput,
} from "@ionic/vue";
import { defineComponent } from "vue";
import { useRouter } from "vue-router";

export default defineComponent({
  components: {
    IonCard,
    IonCardContent,
    IonCardHeader,
    IonCardSubtitle,
    IonCardTitle,
  }
  // setup(){
  //   const router = useRouter();
  //   return {router};
  // },
});
</script>
