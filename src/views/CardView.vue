<template>
    <v-container :fluid=true>
        <h1 class="text-green-darken-4">Card</h1>
        <v-row>
            <v-col>
                <!-- Forma 1-->
                <v-card title="Mi título" color="dark" subtitle="Subtítulo"
                    text="Texto"></v-card>
            </v-col>

            <v-col>
            <!-- Forma 2 -->
                <v-card>
                    <v-img src="../assets/logo.png" height="200" cover></v-img>
                        <v-card-title>Título</v-card-title>
                        <v-card-subtitle>Subtítulo</v-card-subtitle>
                        <v-card-text>
                        Contenido de la tarjeta
                        </v-card-text>
                        <v-card-actions>
                            <v-btn icon="mdi-heart" color="red"></v-btn>
                            <v-btn icon="mdi-share" color="blue"></v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: 'CardView'
}
</script>