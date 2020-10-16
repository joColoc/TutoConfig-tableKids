<template>
  <q-page>
    <h4 class="q-pa-lg text-center">les Cables et plaques</h4>
    <div class="flex-center q-pa-lg row items-start q-gutter-md">
      <!-- <q-card class="my-card">
        <q-img src="~assets/login.jpg" basic> </q-img>
      </q-card>-->
      <q-card class="my-card">
        <q-img src="~assets/google.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-md">
          Cliquez sur connecter avec GOOGLE
        </p>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/indice.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-md">Mettre comme indice impair</p>
      </q-card>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/motdepasse"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/autorisation"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "CompteKiddoware"
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 750px
</style>