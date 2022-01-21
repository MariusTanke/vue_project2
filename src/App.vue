<template>

  <div id="app" class="container">
    <div class="row">
      <div class="col-md-12">
        <h1>Personas</h1>
      </div>
    </div>

    <div class="row">

      <div class="col-md-12">
        <tabla-personas v-bind:personas="personas" />
      </div>

      <div class="col-md-12">
        <cards-personas v-bind:personas="personas" />
      </div>

      <div class="col-md-12" style="margin-top: 20px">
        <formulario />
      </div>
    </div>

  </div>
</template>

<script>
  import TablaPersonas from '@/components/TablaPersonas.vue'
  import CardsPersonas from '@/components/CardsPersonas.vue'
  import formulario from '@/components/formulario.vue'

  
export default {
    name: 'app',
    components: {
      TablaPersonas,
      CardsPersonas,
      formulario,
    },
    data() {
      return {
        personas: [
          {
            id: 1,
            nombre: 'Jon',
            apellido: 'Nieve',
            email: 'jon@email.com',
          },
          {
            id: 2,
            nombre: 'Tyrion',
            apellido: 'Lannister',
            email: 'tyrion@email.com',
          },
          {
            id: 3,
            nombre: 'Daenerys',
            apellido: 'Targaryen',
            email: 'daenerys@email.com',
          },
          {
            id: 4,
            nombre: 'Marius',
            apellido: 'Tankelevicius',
            email: 'tankee265@gmail.com',
          },
        ],
      }
    },
  }
</script>

<style>
  button {
    background: #009435;
    border: 1px solid #009435;
  }
</style>