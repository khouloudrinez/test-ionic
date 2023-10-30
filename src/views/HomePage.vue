<template>
  <ion-page>
    <ion-header>
      <Navbar> </Navbar>
    </ion-header>
    <ion-content>
      <ion-toolbar>
        <div class="header-text">
          <h1 class="is-size-3 has-text-weight-bold">
            Finissez vos démarches administratives avant la tombée de la nuit
          </h1>
          <ion-button fill="outline" size="large" class="red-button">
            Créer mon compte
          </ion-button>
          <ion-img src="/gif.gif" alt="GIF Image" class="gif-image"> </ion-img>
        </div>
        <ion-title class="mt-4">Toutes les procédures:</ion-title>
      </ion-toolbar>
    
    
      <div class="card-container">
        <ion-row>
          <ion-col size="12" size-md="6" size-lg="4" v-for="item in cardData" :key="item.id">
            <ion-card>
              <ion-card-header>
                <ion-card-title>{{ item.title }}</ion-card-title>
              </ion-card-header>
              <ion-card-content>{{ item.content }}</ion-card-content>
            </ion-card>
          </ion-col>
        </ion-row>
      </div>
      <ion-footer>
    
 <Footer></Footer>
  </ion-footer>
    </ion-content>
    
   
  </ion-page>
   
</template>



<script setup>
import Navbar from './Navbar.vue'; import Footer from './Footer.vue';
import { ref } from 'vue';
import {
  IonHeader,
  IonButton,
  IonImg,
  IonTitle,
  IonToolbar,
  IonCardTitle,
  IonCardHeader,
  IonCardContent,
  IonCard,
  IonCol,
  IonRow,
  IonContent,
  IonFooter,
  IonPage,
  IonButtons,
} from '@ionic/vue';
const cardData = ref([
  { id: 1, title: 'Envoi de l’argent Western Union', content: 'Office national des postes' },
  { id: 2, title: 'e-Bawaba - Service administratif', content: 'Ministre des technologies de la communication' },
  { id: 3, title: 'Obtenir le Permis de conduire international tunisien', content: '' },
  { id: 4, title: 'Paiement en ligne du péage (Télépéage)', content: 'Société Tunisie Autoroutes' },
  { id: 5, title: 'Obtention de la carte d’identité nationale (modification de données)', content: 'Ministére de l’intérieur' },
  { id: 6, title: 'Attestation de résidence', content: 'poste de la police' },
  { id: 7, title: 'Obtention d’une Attestation d’origine', content: 'chambre de commerce' },
  { id: 8, title: 'Obtention d’un prêt personnel CNRPS', content: 'caisse national de retraite' },
]);
</script>

<style scoped>
   .card-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
  }

  ion-card {
    min-width: 200px; 
    margin: 10px;
  }
  .red-button {
 
  --color: red;
  --border-color: red;
  --border-radius:10px;
  --font-size: 5px
}
.mt-4 {
  margin-top: 3rem; 
}

.header-text {
  margin-top: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center; 
  text-align: center; 
  margin-bottom: 3rem; 
}
.gif-image {
  display: block;
  margin-top: 30px;
  max-width: 30%; 
  
}


  
</style>