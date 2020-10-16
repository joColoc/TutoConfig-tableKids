<template>
  <q-page>
    <h4 class="q-pa-lg text-center">Autorisation et bloquage</h4>
    <div class="flex-center q-pa-lg row items-start q-gutter-md">
      <q-card class="my-card">
        <q-img src="~assets/autorisation-kp-2.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-sm">
          Autoriser Kid's Place pour qu'il soit en mode activé
        </p>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/blocage.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-sm">
          Cliquez sur connecter avec GOOGLE
        </p>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/autorisation-kp.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-sm">Mettre comme indice impair</p>
      </q-card>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/compteKiddoware"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/save"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "Autorisation"
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 600px
</style>