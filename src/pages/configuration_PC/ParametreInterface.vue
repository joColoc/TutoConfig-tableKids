<template>
  <q-page>
    <h4 class="q-pa-lg text-center">Fixation des cables et mini pc</h4>
    <div class="flex-center q-pa-md row items-start q-gutter-md">
      <q-card class="my-card">
        <q-img src="~assets/interface.jpg" basic> </q-img>

        <q-card-section>
          <p style="font-size:17px" class="text-center">
            "Selectionner le papier peint et aprés avois mis la clé USB avec le
            bon fond d'écran , ou aprés avoir recuperer l'image sur le drive .
            Appliquer le fond d'écran et retourner au parametres "
          </p>
        </q-card-section>
      </q-card>
    </div>

    <!--button-->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/parametreAvances"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/gestionutilisateur"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "ParametreInterface",
  data() {
    return {};
  }
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 900px
</style>