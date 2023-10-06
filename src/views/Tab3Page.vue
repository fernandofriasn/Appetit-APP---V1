<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>User info</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 3</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-card color="dark">
        <img
          alt="Silhouette of mountains"
          src="https://ionicframework.com/docs/img/demos/card-media.png"
        />
        <ion-card-header>
          <ion-card-title>Fernando Frias</ion-card-title>
          <ion-card-subtitle>Premium User</ion-card-subtitle>
        </ion-card-header>

        <!-- <ion-card-content>
        Here's a small text description for the card content. Nothing more, nothing less.
        </ion-card-content> -->
      </ion-card>

      <ion-list>
        <ion-item>
          <ion-input label="Name" placeholder="Fernando Frias"></ion-input>
        </ion-item>

        <ion-item>
          <ion-input
            label="Password"
            type="password"
            value="password"
          ></ion-input>
        </ion-item>

        <ion-item>
          <ion-input
            label="Email"
            type="email"
            placeholder="ffrias@domain.com"
          ></ion-input>
        </ion-item>

        <ion-item>
          <ion-input
            label="Telephone"
            type="tel"
            placeholder="809-888-8888"
          ></ion-input>
        </ion-item>

        <ion-item>
          <ion-input
            label="Credit Card"
            type="text"
            placeholder="Visa/Mastercard (Optional)"
          ></ion-input>
        </ion-item>

      </ion-list>

      <br>
      <br>
      <br>
      

      <ion-button expand="full" color="success">Update Account</ion-button>
      <ion-button expand="full" color="danger">Delete Account</ion-button>

    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
} from "@ionic/vue";
import ExploreContainer from "@/components/ExploreContainer.vue";
</script>
