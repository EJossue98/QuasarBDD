<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar>


       
      </q-toolbar>
      <div class="q-px-lg q-pt-xl q-mb-md text-center">
        <div class="text-h3">APLICACIÓN LISTA DE COSAS POR HACER</div>
      </div>
    </q-header>

      <q-footer class="bg-white" bordered>
      <q-tabs class="text-grey-10" active-color="primary" indicator-color="primary">
        <q-route-tab name="Camera" icon="home" label="Home" to="/home" exact/>
        <q-route-tab name="Lista" icon="mail" label="Lista" to="/" exact/>

      </q-tabs>
      </q-footer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import EssentialLink from 'components/EssentialLink.vue'
import { date } from 'quasar'

export default {
  name: 'MainLayout',
  components: { EssentialLink },
  data () {
    return {
      leftDrawerOpen: false,
      essentialLinks: linksData
    }
  },
}
</script>