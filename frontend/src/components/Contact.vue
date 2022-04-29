<template>
    <div>
        <div class="grey darken-4 pb-2 pt-16">
            <h1 class="font-color font-weight-light text-center">Contact Information</h1>
        </div>
        <v-row class="grey darken-4 ma-0 pr-lg-16 pl-lg-16">
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-end pr-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text class="text-center">
                        <h2 class="font-color pa-0 pb-3"><v-icon class="font-color mr-2">mdi-phone</v-icon>Contact Number</h2>
                        <v-divider class="mb-3 test"></v-divider>
                        <h3 class="font-color font-weight-light">
                            +639244466666
                        </h3>
                    </v-card-text>
                </v-card>
            </v-col>
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pl-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text class="text-center">
                        <h2 class="font-color pa-0 pb-3"><v-icon class="font-color mr-2">mdi-email</v-icon>Email</h2>
                        <v-divider class="mb-3 test"></v-divider>
                        <h3 class="font-color font-weight-light">
                            emranpendaliday1010@gmail.com
                        </h3>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
        <v-row class="grey darken-4 ma-0 pr-lg-16 pl-lg-16 pb-16">
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-end pr-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text class="text-center">
                        <h2 class="font-color pa-0 pb-3"><v-icon class="font-color mr-2">mdi-map-marker</v-icon>Address</h2>
                        <v-divider class="mb-3 test"></v-divider>
                        <h3 class="font-color font-weight-light px-2 text-div">
                            Casa Mira South, Pitalo, San Fernando, Cebu, Philippines 6018
                        </h3>
                    </v-card-text>
                </v-card>
            </v-col>
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pl-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text class="text-center">
                        <h2 class="font-color pa-0 pb-3"><v-icon class="font-color mr-2">mdi-web</v-icon>Social Media</h2>
                        <v-divider class="mb-3 test mb-4"></v-divider>
                        <v-icon class="font-color" large>mdi-facebook</v-icon>
                        <v-icon class="font-color mx-2" large>mdi-discord</v-icon>
                        <v-icon class="font-color" large>mdi-linkedin</v-icon>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
    </div>
</template>
<style scoped>
    .font-color {
        color: #E0E0E0;
        font-family: "Roboto";
        font-weight: 400;   
    }
    .test {
        background: #E0E0E0;
    }
    .text-div {
        line-height: 1.6;
    }
</style>