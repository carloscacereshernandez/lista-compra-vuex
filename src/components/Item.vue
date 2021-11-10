<template>
<span>
  <strong>{{nombre}}</strong> 
  ({{cantidad}} {{unidades}})
</span>
</template>

<script>
export default {
  name: "Item",
  props: ['id', 'nombre', 'cantidad', 'unidades']
};
</script>