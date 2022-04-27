<template>
    <v-container class="my-15">
        <v-row justify="center">
            <v-col lg="12" class="text-center">
                <v-subheader class="text-h4 justify-center">
                    Contact Us
                </v-subheader>

                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>

            </v-col>

            <v-col lg="6">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d7864452.3833377445!2d101.4132682470241!3d15.747719357779795!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31157a4d736a1e5f%3A0xb03bb0c9e2fe62be!2zVmnhu4d0IE5hbQ!5e0!3m2!1svi!2s!4v1650966278704!5m2!1svi!2s" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </v-col>

            <v-col lg="6">
                <v-form ref="form">
                    <v-text-field
                            v-model="contactInfo.name"
                            :counter="10"
                            label="Name"
                            required
                    ></v-text-field>

                    <v-text-field
                            v-model="contactInfo.email"
                            label="E-mail"
                            required
                    ></v-text-field>

                    <v-textarea label="Message" v-model="contactInfo.message">

                    </v-textarea>

                    <v-btn color="success" class="mr-4">
                        Send
                    </v-btn>
                </v-form>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        name: "Contactus",
        data(){
            return{
                contactInfo:{

                }
            }
        }
    }
</script>

<style scoped>

</style>