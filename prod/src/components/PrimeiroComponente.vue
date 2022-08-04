<template>
<div>
    <MultiplosEventos></MultiplosEventos>
    <!-- componentes independentes, pode ser utilizados por exemplos para adicionar produtos para o carinho -->
    <ReutilizacaoComp></ReutilizacaoComp>
        <ReutilizacaoComp></ReutilizacaoComp>
            <ReutilizacaoComp></ReutilizacaoComp>
            <ImagemComponente></ImagemComponente>
</div>
</template>

<script>
import MultiplosEventos from './multiplosEventos.vue'
import ReutilizacaoComp from './reutilizacaoComp.vue'
import ImagemComponente from './imagemComponente.vue'
export default {
  name: 'PrimeiroComponente',
  data () {
    return {
      nome: 'beatriz',
      profi: 'programa'
    }
  },
  components: { MultiplosEventos, ReutilizacaoComp, ImagemComponente }
}
</script>
