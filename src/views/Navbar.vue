<template>
    
      <ion-toolbar class="header">
       
        <ion-buttons slot="start">
          <ion-button>
            <img src="/idaraty_logo_txt_fr.png" alt="Idaraty - ادارتي" class="logo">

          </ion-button>
        </ion-buttons>
        <ion-title>
          <ion-button class="button" fill="outline">
            <span>بالتونسي</span>
          </ion-button>
        </ion-title>
   <ion-buttons slot="end">
            <ion-button color="danger" class="red-button">
    Plus
  </ion-button>
    
        </ion-buttons>
      </ion-toolbar>
   
  </template>
  
  <script>
  export default {
    components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonButtons,
    IonButton,
  
  },
    name: 'Navbar',
  };
  import { IonHeader, IonToolbar, IonTitle, IonButtons, IonButton } from '@ionic/vue';
  </script>
  
  <style scoped>
  
  .header {
    --background: #000; 
    --border-color: transparent; 
    --color: #fff; 
  }
  
  .button {
    --border-color: #fff; 
    --color: #fff; 
  }
  .red-button {
    --background: rgb(230, 54, 54); 
    --color: white; 
    
  }
  .logo {
    width: 130px; 
    height: auto; 
  }
  </style>
  