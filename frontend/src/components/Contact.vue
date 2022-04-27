<template>
    <div>
        <div class="grey darken-4 pb-2 pt-16">
            <h1 class="font-color font-weight-light text-center">Contact Information</h1>
        </div>
        <v-row class="grey darken-4 ma-0 pr-lg-16 pl-lg-16">
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-end pr-lg-16 pt-5">
                <v-card
                    class="pa-3 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text class="text-center">
                        <h2 class="font-color pa-0 pb-3">Contact Number</h2>
                        <v-divider class="mb-3 test"></v-divider>
                        <h2 class="font-color font-weight-light">
                            +639244466666
                        </h2>
                    </v-card-text>
                </v-card>
            </v-col>
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pl-lg-16 pt-5">
                <v-card
                    class="pa-3 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text class="text-center">
                        <h2 class="font-color pa-0 pb-3">Email</h2>
                        <v-divider class="mb-3 test"></v-divider>
                        <h2 class="font-color font-weight-light">
                            emranpendaliday1010@gmail.com
                        </h2>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
        <v-row class="grey darken-4 ma-0 pb-16 pr-lg-16 pl-lg-16">
            <v-col cols="12" md="12" class="d-flex justify-center pt-5">
                <v-card
                    class="pa-3 grey darken-4"
                    width="800"
                    flat
                >
                    <v-card-text class="text-center">
                        <h2 class="font-color pa-0 pb-3">Address</h2>
                        <v-divider class="mb-3 test"></v-divider>
                        <h2 class="font-color font-weight-light px-2 text-div">
                            Lawaan 1, Talisay city, Cebu, PhilippinesLawaan 1, Talisay city, Cebu, Philippines
                        </h2>
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