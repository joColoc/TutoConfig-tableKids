<template>
  <q-page>
    <h4 class="q-pa-lg text-center">Fixation des cables et mini pc</h4>
    <div class="flex-center q-pa-lg row items-start q-gutter-md">
      <q-card class=" my-card">
        <q-img src="~assets/plaque-cable.jpg" basic> </q-img>

        <q-card-section class="text-center">
          <p style="font-size:17px">Fixation des cables</p>
        </q-card-section>
      </q-card>
      <q-card class=" my-card">
        <q-img src="~assets/miniPC.jpg" basic> </q-img>

        <q-card-section class="text-center">
          <p style="font-size:17px">
            Fixation de l'accroche de l'ordinateur avec mise en place du mini PC
          </p>
        </q-card-section>
      </q-card>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/cables"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/positionAdhésif"
      />
      <br />
    </div>
  </q-page>
</template>
  </q-page>
  
</template>

<script>
export default {
  name: "FixationCables",
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