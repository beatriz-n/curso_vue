<template>
    <div>
        <button @click="primeiro(txt1,$event), segundo(txt2,$event)">Ativar multiplos eventos</button>
    </div>
</template>

<script>
export default {
  name: 'multiplosEventos',
  data () {
    return {
      multiplos_eventos: '',
      txt1: 'primeiro evento',
      txt2: 'segundo evento'
    }
  },
  methods: {
    primeiro (e) {
      this.multiplos_eventos = 'primeiro evento ativado'
    }
  }
}
</script>

<style scoped>
div{
    margin: 100px;
}
</style>
