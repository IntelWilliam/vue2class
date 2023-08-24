<template>
  <div id="app">
    <ul class="list-group">
      <li v-for="(ide, index) in ides" @click="suma(index)" :key="ide.id"
        class="list-group-item d-flex justify-content-between align-items-center">
          {{ index }} --- {{ ide.nombre }}
        <span class="badge badge-primary badge-pill">{{ ide.voto }}</span>
      </li>
      
    </ul>
  </div>
</template>


<script>
import { mapMutations, mapState } from 'vuex';

export default {
  name: 'ListaHome',

  computed: {
    ...mapState(['ides'])
  },
 
  methods: {
    ...mapMutations(['suma'])
  },

}
</script>