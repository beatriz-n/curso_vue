<template>
    <h1>meu nome é: {{nome}}</h1>
</template>

<script>
export default {
  nome: 'LifeCycle',
  data () {
    return {
      nome: 'Goku'
    }
  },
  created () {
    setTimeout(() => {
      this.nome = 'Vegeta'
    }, 1000)
    this.lifeCycle()
  },
  mounted () {
    setTimeout(() => {
      this.nome = 'Frezza'
    }, 2000)
  },
  methods: {
    lifeCycle () {
      console.log('executou')
    }
  }
}
// eventos acontecendo em determinadas etapas
</script>
