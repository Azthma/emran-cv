<template>
    <div>
        <div class="grey darken-4 pb-3 pt-16">
            <h1 class="font-color font-weight-light text-center">About Me</h1>
        </div>
        <v-col class="d-flex justify-center pa-lg-0 card-col" >
            <v-card class="rounded-0 mb-16" max-width="1000" flat>
                <div class="text-div grey darken-4 font-color font-weight-light text-center">
                        Hello! I'm Emran Pendaliday. I am a Web Developer and Quality Assurance Specialist. I am Back-end Developer and Front-end Developer 
                        and is skilled in Node js Express for my back-end development and Vue js for my front-end development. I am proficient in Mocha js which I 
                        use in my api testing and Selenium C# for my front-end automated testing. I am a quick learner and a fast worker.
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
                            Develop websites and web application as a full stack developer. Ensures that the website and web application is visually appealing and user friendly.
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
                            I do API testing and SQL testing for back-end testing and automated testing for the overall functionality of the web application for front-end testing.
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
                            manage computer-based information systems and solve technical and application problems.
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