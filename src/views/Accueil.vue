<template>
  <div>
    <div class="logo_container">
      <img alt="Logo du groupe Cold Lemonade" class="logo" src="@/assets/img/cold_lim_logos/orange_bleu.png">
    </div>
    <YoutubeVideo/>
    <SocialNetworks/>
  </div>

</template>

<script lang="ts">
import {defineComponent} from 'vue';
import SocialNetworks from "@/components/SocialNetworks.vue";
import YoutubeVideo from "@/components/YoutubeVideo.vue";

export default defineComponent({
  name: 'Accueil',
  components: {YoutubeVideo, SocialNetworks}
});
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Satisfy&display=swap');
@import "~@/assets/scss/main.scss";

.logo_container {
  padding-top: 5%;
  display: flex;
  justify-content: flex-end;
  padding-right: 5%;
  align-items: center;

  @media (min-width: 600px) {
    justify-content: center;
    padding-top: 1%;
    padding-right: 0;
  }

  .logo {
    height: 50px;

    @media (min-width: $breakpoint-sm) {
      height: 100px;
    }
  }
}

</style>
