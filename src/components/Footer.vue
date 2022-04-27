<template>
    <v-footer padless >
        <v-col lg="12">
            <v-row justify="center">
                <v-col lg="4" class="text-center">
                    <v-toolbar-title>Web Burden</v-toolbar-title>
                    <v-card-text>
                        <v-btn
                                v-for="icon in icons"
                                :key="icon"
                                class="mx-4 black--text"
                                icon
                        >
                            <v-icon size="24px">
                                {{ icon }}
                            </v-icon>
                        </v-btn>
                    </v-card-text>

                    <v-subheader>
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ipsam suscipit deleniti minus repellendus ipsum natus amet beatae facilis ab aut quod quo magnam doloribus, error cum minima! Nostrum, at inventore.
                    </v-subheader>

                    <v-form class="mt-4">
                        <v-text-field label="Email" outlined dense />
                        <v-btn rounded color="success">Subscribe us</v-btn>
                    </v-form>
                </v-col>
            </v-row>
            <div class="mt-10">
                <v-divider></v-divider>
                <v-subheader>
                    © Copyright Web Burden. All Rights Reserved.  {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
                    <v-spacer />
                    <strong>Designed by Hieu</strong>
                </v-subheader>
            </div>
        </v-col>

    </v-footer>
</template>

<script>
    export default {
        name: "Footer",
        data(){
            return{
                icons: [
                    'mdi-facebook',
                    'mdi-twitter',
                    'mdi-linkedin',
                    'mdi-instagram',
                ],
            }
        }
    }
</script>

<style scoped>
    .v-toolbar__title{
        font-size: 32px;
        color: #4caf50;
        font-weight: 700;
        font-family: cursive;
    }
</style>