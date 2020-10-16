<template>
  <q-page>
    <h4 class="q-pa-lg text-center">Fixation des cables et mini pc</h4>
    <div class="flex-center q-pa-lg row items-start q-gutter-md">
      <q-card class="my-card">
        <q-img src="~assets/alim.jpg" basic> </q-img>
      </q-card>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/adhésifDeProtection"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/miseEnPlace"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "VerficationCables",
  data() {
    return {};
  }
};
</script>


<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 750px
</style>