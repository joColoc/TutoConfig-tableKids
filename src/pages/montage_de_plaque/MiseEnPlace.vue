<template>
  <q-page>
    <h4 class=" text-center">Fixation des cables et mini pc</h4>

    <div class="flex-center flex flex-center items-start q-gutter-md">
      <q-card class=" q-my-lg flex flex-center my-cardA">
        <q-img src="~assets/table-dessous.jpg" basic> </q-img>
        <p class="text-center q-ma-md text-h6">Mise en place de la table</p>
      </q-card>
    </div>
    <div class="flex-center flex flex-center items-start q-gutter-md">
      <q-card class=" my-card">
        <q-img src="~assets/table-dessous-2.jpg" basic> </q-img>
        <p class="q-py-sm text-center q-ma-md">
          Mise en place des vises de serrage en diagonale pour ne pas forcer sur
          la structure
        </p>
      </q-card>
      <q-card class=" my-card">
        <q-img src="~assets/table-dessous-3.jpg" basic> </q-img>
        <p style="font-size:17px" class="text-center q-ma-lg q-py-sm">
          Accroche des câbles à la table
        </p>
      </q-card>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/verificationCables"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label=" Configuration Mini PC  "
        to="/configBase"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "MiseEnPlace",
  data() {
    return {};
  }
};
</script>
<style lang="sass" scoped>
.my-cardA
  display : block
  width: 100%
  max-width: 600px

.my-card
  width: 100%
  max-width: 400px
</style>