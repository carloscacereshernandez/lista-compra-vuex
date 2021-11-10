<template>
  <div>
    <ul class="listaItems">
      <li v-for="i in lista" :key="i.id">
        <item :nombre="i.nombre" 
              :cantidad="i.cantidad"
              :unidades="i.unidades"
              :id="i.id"/>
      </li>
    </ul>
  </div>
</template>

<script>
import Item from './Item'

export default {
  name: "ListaItems",
  components: {
    Item
  },
  computed: {
    lista: function() {
      return this.$store.state.lista;
    }
  }
};
</script>

<style scoped>
.listaItems {
  text-align: left;
}
</style>
