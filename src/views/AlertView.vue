<template>
   <v-container :fluid=true>
        <h1 class="text-green-darken-4">Alerta</h1>
        <!-- Botón -->
        <v-btn
        prepend-icon="mdi-bell-ring"
        color="indigo"
        rounded="xl"
        @click="alertState = true">Mostrar alerta</v-btn>
        <br>
        <br>
        <!-- Alerta -->
        <v-alert
        closable
        v-model="alertState"
        icon="mdi-information"
        title="Respuesta"
        text="El producto ha sido guardado"
        type="info"
        ></v-alert>
    </v-container>
</template>
<script>
export default {
    name: 'AlertView',
    data(){
        return {
            alertState: false
        }
    }

}
</script>