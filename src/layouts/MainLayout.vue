<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          v-on:click="leftDrawerOpen = !leftDrawerOpen"
          class="q-pa-md"
        />

        <q-toolbar-title>
          Table kids
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      content-class="bg-grey-1"
    >
      <q-expansion-item class="q-pt-lg" icon="pages" label="Montage de plaque">
        <q-list>
          <MontagePlaqueComponents
            v-for="link in menuJsonMontageDePlaque"
            :key="link.title"
            v-bind="link"
          />
        </q-list>
      </q-expansion-item>

      <q-expansion-item
        class="q-pt-lg"
        icon="pages"
        label="Configuration Mini PC"
      >
        <q-list class="q-pl-lg">
          <q-item to="/configBase">
            <q-item-section avatar>
              <q-icon name="check" />
            </q-item-section>
            <q-item-section>
              <q-item-label>Configuration de base</q-item-label>
            </q-item-section>
          </q-item>
          <q-expansion-item icon="check" label="contrôle parental">
            <q-list class="q-pl-lg">
              <q-item to="/motdepasse" class="q-pl-lg">
                <q-item-section avatar>
                  <q-icon name="check" />
                </q-item-section>
                <q-item-section>
                  <q-item-label> Mot de passe </q-item-label>
                </q-item-section>
              </q-item>
              <q-item to="/compteKiddoware" class="q-pl-lg">
                <q-item-section avatar>
                  <q-icon name="check" />
                </q-item-section>
                <q-item-section>
                  <q-item-label> Lier le compte kiddoware </q-item-label>
                </q-item-section>
              </q-item>
              <q-item to="/autorisation" class="q-pl-lg">
                <q-item-section avatar>
                  <q-icon name="check" />
                </q-item-section>
                <q-item-section>
                  <q-item-label> Autorisitation et bloquage </q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-expansion-item>
          <q-item to="/save">
            <q-item-section avatar>
              <q-icon name="check" />
            </q-item-section>
            <q-item-section>
              <q-item-label> Sauvegarde et restauration</q-item-label>
            </q-item-section>
          </q-item>
          <q-expansion-item icon="check" label="Paramètres">
            <q-list class="q-pl-lg">
              <q-item to="/parametres" class="q-pl-lg">
                <q-item-section avatar>
                  <q-icon name="check" />
                </q-item-section>
                <q-item-section>
                  <q-item-label> Contrôle parental</q-item-label>
                </q-item-section>
              </q-item>
              <q-item to="/parametreAvances" class="q-pl-lg">
                <q-item-section avatar>
                  <q-icon name="check" />
                </q-item-section>
                <q-item-section>
                  <q-item-label> Paramètres avancés </q-item-label>
                </q-item-section>
              </q-item>
              <q-item to="/parametreInterface" class="q-pl-lg">
                <q-item-section avatar>
                  <q-icon name="check" />
                </q-item-section>
                <q-item-section>
                  <q-item-label> Paramètres interface </q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-expansion-item>
          <q-item to="/gestionutilisateur">
            <q-item-section avatar>
              <q-icon name="check" />
            </q-item-section>
            <q-item-section>
              <q-item-label> Gestion Utilisateur</q-item-label>
            </q-item-section>
          </q-item>
          <q-item to="/extinction">
            <q-item-section avatar>
              <q-icon name="check" />
            </q-item-section>
            <q-item-section>
              <q-item-label> Extinction</q-item-label>
            </q-item-section>
          </q-item>
          <q-item to="/verification">
            <q-item-section avatar>
              <q-icon name="check" />
            </q-item-section>
            <q-item-section>
              <q-item-label>Verfication configuration </q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-expansion-item>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import MontagePlaqueComponents from "components/MenuMontagePlaque.vue";

const montageDePlaque = [
  {
    title: "Materiels",
    icon: "check",
    to: "/materiels"
  },
  {
    title: "Plaques & cables",
    icon: "check",
    to: "/cables"
  },
  {
    title: "Fixation des câbles et mini PC",
    icon: "check",
    to: "/fixationCables"
  },
  {
    title: "Positionnement adhésif",
    icon: "check",
    to: "/positionAdhésif"
  },
  {
    title: "Collage alimentation de l'écran",
    icon: "check",
    to: "/collage"
  },
  {
    title: "Adhésif de protection",
    icon: "check",
    to: "/adhésifDeProtection"
  },
  {
    title: "Vérification cablages du mini PC",
    icon: "check",
    to: "/verificationCables"
  },
  {
    title: "Mise en place | Accroche des câbles",
    icon: "check",
    to: "/miseEnPlace"
  },
  {
    title: "Exemple de tiroir",
    icon: "check",
    to:"",
    multi:[
    {
      title: "Exemple 1",
      icon: "check",
      to: "/miseEnPlace"
    },
    {
      title: "Exemple 2",
      icon: "check",
      to: "/verificationCables"
    },
    ],
  },
]

export default {
  name: "MainLayout",
  components: { MontagePlaqueComponents },
  data() {
    return {
      leftDrawerOpen: false,
      menuJsonMontageDePlaque: montageDePlaque
    };
  }
};
</script>
