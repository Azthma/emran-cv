<template>
    <div>
        <div class="grey darken-4 pb-3 pt-16">
            <h1 class="font-color font-weight-light text-center">About Me</h1>
        </div>
        <v-col class="d-flex justify-center pa-lg-0 card-col" >
            <v-card class="rounded-0 mb-16" max-width="1000" flat>
                <div class="text-div grey darken-4 font-color font-weight-light text-center">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et 
                        dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip 
                        ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu 
                        fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt 
                        mollit anim id est laborum.
                </div>
            </v-card>
        </v-col>
        <div class="grey darken-4 pb-2 pt-16">
            <h1 class="font-color font-weight-light text-center">What I Do</h1>
        </div>
        <v-row class="grey darken-4 ma-0 px-0 px-lg-16">
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-end pr-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text>
                        <v-card-title class="font-color pa-0 pb-3">Web Development</v-card-title>
                        <v-divider class="mb-3 test"></v-divider>
                        <div class="font-color">
                            Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, 
                            totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae 
                            dicta sunt explicabo.
                        </div>
                    </v-card-text>
                </v-card>
            </v-col>
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pl-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text>
                        <v-card-title class="font-color pa-0 pb-3">Unit Testing</v-card-title>
                        <v-divider class="mb-3 test"></v-divider>
                        <div class="font-color">
                            Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur 
                            magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem 
                            ipsum quia dolor sit amet, consectetur, adipisci velit.
                        </div>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
        <v-row class="grey darken-4 ma-0 pb-16 pr-lg-16 pl-lg-16">
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-end pr-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text>
                        <v-card-title class="font-color pa-0 pb-3">IT Support</v-card-title>
                        <v-divider class="mb-3 test"></v-divider>
                        <div class="font-color">
                            Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, 
                            nisi ut aliquid ex ea commodi consequatur?
                        </div>
                    </v-card-text>
                </v-card>
            </v-col>
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pl-lg-16 pt-5">
                <v-card
                    class="pa-1 grey darken-4"
                    width="400"
                    flat
                >
                    <v-card-text>
                        <v-card-title class="font-color pa-0 pb-3">Lorem Ipsum</v-card-title>
                        <v-divider class="mb-3 test"></v-divider>
                        <div class="font-color">
                            Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae 
                            consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur
                        </div>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
    </div>
</template>
<style scoped>
    .font-color {
        color: #E0E0E0;
    }
    .test {
        background: #E0E0E0;
    }
    .card-col{
        background-color: #212121 !important;
    }
    .text-div {
         line-height: 1.6;
    }
</style>