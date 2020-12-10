<template>
    <v-container class="container">
        <ul>
           <v-row>
                <v-col
                v-for="n in 12"
                :key="n"
                class="d-flex child-flex"
                cols="4"
                >
                <v-card>
                <v-img
                    :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                    :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
                    aspect-ratio="1"
                    class="grey lighten-2"
                >
                    <template v-slot:placeholder>
                    <v-row
                        class="fill-height ma-0"
                        align="center"
                        justify="center"
                    >
                        <v-progress-circular
                        indeterminate
                        color="grey lighten-5"
                        ></v-progress-circular>
                    </v-row>
                    </template>
                </v-img>
                 <v-card-subtitle size="1">
                             <p class="text-caption"> Lorem ipsum </p>
                    </v-card-subtitle>
                </v-card>
                </v-col>
            </v-row>
        </ul>
    </v-container>
</template>

<script>
export default {
    name:"FotosIndex",
 /*   data(){
        return{
            imagens:[
                {
                id: 1,
                foto: "https://picsum.photos/500/300", 
                texto: "Lorem Ipsum",
                }
            ]
        }
    }*/
}
</script>

<style scoped>
.container{
    display: flex;
    justify-content: center;
}
/*.fotos{
   width: 50vw;
    display: flex;
    justify-content: center;
    background-color: aqua;
}*/
</style>