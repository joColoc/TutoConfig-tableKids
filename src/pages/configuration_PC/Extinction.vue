<template>
  <q-page>
    <h4 class="q-pa-lg text-center">Extinction</h4>
    <div class="flex-center q-pa-lg row items-start q-gutter-md">
      <q-card class="my-card">
        <q-img src="~assets/shutdown-2.jpg" basic> </q-img>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/shutdown-3.jpg" basic> </q-img>
      </q-card>
      <q-card-section>
        <p class="" style="font-size:17px">
          Puis configurer l'exinction automatique de la table. <br />
          Pour se faire, se rendre dans l'application shutdown
          <img src="~assets/shutdown.jpg" alt="button-shutdown" width="5%" />
          qui est en dehors du contrôle parental, puis régler sur
          <strong>20H30</strong>
        </p>
      </q-card-section>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/gestionutilisateur"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/verification"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "Extinction"
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 750px
</style>