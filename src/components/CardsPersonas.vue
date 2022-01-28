<template>

    <div>

        <div class="row">

            <div class="col-12 col-sm-6 col-md-4 col-lg-3" v-for="persona in personas" :key="persona.id">

                <div class="card" style="border: solid 3px lightblue">

                    <div class="card-body">
                        <h5 class="card-title text">ID: {{ persona.id}}</h5>
                        <p class="card-text">Nombre: {{ persona.nombre}}</p>
                        <p class="card-text">Apellido: {{ persona.apellido}}</p>
                        <p class="card-text">Email: {{ persona.email}}</p>
                    </div>

                </div>

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