<template>
    <ion-footer class="ion-padding">
      <div class="ion-text-center logo-container">
        <img src="/idaraty_logo_txt_fr.png" alt="Idaraty.tn" class="logo">
      </div>
      <div class="ion-text-center social-icons">
        <a :href="facebookLink" target="_blank" rel="noopener" title="Idaraty sur Facebook">
          <img src="/facebook.png" alt="Facebook" class="icon-link">
        </a>
        <a :href="twitterLink" target="_blank" rel="noopener" title="Idaraty sur Twitter">
          <img src="/twitter.png" alt="Twitter" class="icon-link">
        </a>
        <a :href="linkedinLink" target="_blank" rel="noopener" title="Idaraty sur Linkedin">
          <img src="/linkedin.png" alt="LinkedIn" class="icon-link">
        </a>
        <a :href="youtubeLink" target="_blank" rel="noopener" title="Idaraty sur Youtube">
          <img src="/youtube.png" alt="LinkedIn" class="icon-link">
        </a>
        <a :href="pinterestLink" target="_blank" rel="noopener" title="Idaraty sur Pinterest">
          <img src="/pinterest.png" alt="LinkedIn" class="icon-link">
        </a>
      </div>
      <div class="ion-text-center ion-text-bold title">
        Nous encore une fois
      </div>
      <div class="ion-text-center">
        Nous développons des plateformes centrées sur les citoyens et des solutions qui intègrent l'expérience utilisateur et la technologie nécessaires pour renforcer la confiance entre les citoyens et les institutions publiques et aboutir à un changement positif en Tunisie.
      </div>
      <div class="ion-text-center ion-text-bold title">
        A toi maintenant
      </div>
      <div class="ion-text-center">
        Jouons à un petit jeu pour briser la glace. Pour commencer, penses à 5 choses que tu aimes particulièrement chez toi. Clique ici quand tu auras fini.
      </div>
    </ion-footer>
  </template>
  
  <script>
  import { IonFooter } from '@ionic/vue';
  
  export default {
    components: {
      IonFooter,
    },
    name: 'Footer',
    data() {
      return {
        facebookLink: "https://www.facebook.com/idaraty.tn",
        twitterLink: "https://twitter.com/Idaraty_tn",
        linkedinLink: "https://www.linkedin.com/company/idaraty-tn/",
        youtubeLink:"https://www.youtube.com/channel/UCgg2ro3bsZ3QnyhGzyOVc1g",
        pinterestLink:"https://www.pinterest.com/idaraty_tn/",
      };
    },
  };
  </script>
  
  <style scoped>
  .logo-container {
    margin-bottom: 20px; /* Add space between logo and social icons */
  }
  
  .logo {
    width: 130px;
    height: auto;
  }
  
  .icon-link {
    margin: 0 10px;
    width: 24px;
    height: 24px;
  }
  
  .title {
    font-size: 20px; /* Adjust the font size as needed */
    font-weight: bold; /* Make the titles bold */
  }
  
  /* Add space between paragraphs */
  ion-footer > div {
    margin-bottom: 10px;
  }
  
  .ion-text-center {
    text-align: center;
  }
  </style>
  