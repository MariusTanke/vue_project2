<template>

    <div class="card-deck">
          
        <div class="card" style="width: 18rem;"  v-for="persona in personas" :key="persona.id">

            <div class="card-body">
                <h5 class="card-title text">ID: {{ persona.id}}</h5>
                <p class="card-text">Nombre: {{ persona.nombre}}</p>
                <p class="card-text">Apellido: {{ persona.apellido}}</p>
                <p class="card-text">Email: {{ persona.email}}</p>
            </div>

        </div>

    </div>
    
</template>

<script>

    export default {

        name: 'cards-personas',
        props: {
            personas: Array,
        },

    }

</script>