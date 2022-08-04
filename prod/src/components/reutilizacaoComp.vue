<template>
    <div>
        <button @click="ativar">clique</button>
        <span v-show="ativou">ativado</span>
    </div>
</template>
<script>
export default {
  name: 'reutilizacaoComp',
  data () {
    return {
      ativou: false
    }
  },
  methods: {
    ativar () {
      this.ativou = !this.ativou
    }
  }
}
</script>,
