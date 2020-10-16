<template>
  <q-page>
    <h4 class="q-pa-lg text-center">les Cables et plaques</h4>
    <div class="flex-center q-pa-lg row items-start q-gutter-md">
      <q-card class="my-card">
        <q-img src="~assets/plaque.jpg" basic> </q-img>
        <p class=" q-pa-sm text-h6 text-center">plaque</p>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/cable1.jpg" basic> </q-img>
        <p class=" q-pa-sm text-h6 text-center">Câbles VGA</p>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/cable2.jpg" basic> </q-img>
        <p class=" q-pa-sm text-h6 text-center">Câbles USB 3</p>
      </q-card>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/materiels"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/fixationCables"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "Cables"
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 500px
</style>