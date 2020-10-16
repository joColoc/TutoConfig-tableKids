<template>
  <div class="q-pa-md">
    <h4 class=" text-center">Autorisation et bloquage</h4>
    <div class="flex-center row items-start q-gutter-md">
      <q-card class="my-card">
        <q-img src="~assets/cp-1.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-sm">
          Autoriser Kid's Place pour qu'il soit en mode activé
        </p>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/cp-2.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-sm">
          Cliquez sur connecter avec GOOGLE
        </p>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/cp-3.jpg" basic> </q-img>
        <p class="text-center text-h6 q-pa-sm">Mettre comme indice impair</p>
      </q-card>
    </div>
    <!-- <p class="text-h6 ">selectionner control parental</p>-->

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/save"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/parametreAvances"
      />
      <br />
    </div>
  </div>
</template>
<script>
export default {
  name: "parametres",
  data() {
    return {};
  }
};
</script>


<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 600px
</style>
