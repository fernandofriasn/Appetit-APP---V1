<template>
    <div class="map" ref="mapDivRef"></div>
  </template>
  
  <script lang="ts">
  import { ref, onMounted } from 'vue';
  
  declare var google: any;
  
  declare global {
    interface Window {
      initMap: () => void;
    }
  }
  
  export default {
    setup() {
      const map = ref(null);
      const mapDivRef = ref(null);
  
      onMounted(() => {
        const key = 'AIzaSyB6dkGZhjNebHFyQ3TTm9Xd1psIeQqk3PY'; // Clave de API
  
        if (!key) {
          console.error('Falta la clave de API de Google Maps.');
          return;
        }
  
        const googleMapScript = document.createElement('script');
        googleMapScript.setAttribute(
          'src',
          `https://maps.googleapis.com/maps/api/js?key=${key}&callback=initMap`
        );
  
        googleMapScript.setAttribute('defer', '');
        googleMapScript.setAttribute('async', '');
        document.head.appendChild(googleMapScript);
  
        googleMapScript.onload = () => {
          document.head.removeChild(googleMapScript);
        };
  
        googleMapScript.onerror = () => {
          console.error('Error al cargar el script de Google Maps.');
        };
      });
  
      window.initMap = () => {
        map.value = new google.maps.Map(mapDivRef.value, {
          center: { lat: 19.462835, lng: -70.662902 }, // Cambia las coordenadas para centrar el mapa
          zoom: 20, // Cambia el nivel de zoom según tus necesidades
        });
      };
  
      return {
        mapDivRef,
      };
    },
  };
  </script>
  
  <style lang="css" scoped>
  .map {
    width: 100%;
    height: 675px;
  }
  </style>