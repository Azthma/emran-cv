<template>
    <v-app>
        <v-main>
            <v-row class="grey darken-3 pt-16 pb-16" no-gutters>
                <v-col cols="12" md="6" class="d-flex justify-center justify-lg-end align-center pr-lg-6 pt-5 pb-5">
                    <v-avatar size="200">
                        <img 
                            style="object-fit: cover;"
                            src="../assets/profile.png"
                        >
                    </v-avatar>
                </v-col>
                <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start align-center pl-lg-6 pt-5 pb-5">
                    <v-row>
                        <v-col cols="12" class="d-flex justify-center justify-lg-start align-center pb-0 font-color">
                            <h1>Lorem Ipsum</h1>
                        </v-col>
                        <v-col cols="12" class="d-flex justify-center justify-lg-start align-center pt-0 font-color">
                            <h2>Finibus Bonorum et Malorum</h2>
                        </v-col>
                    </v-row>
                </v-col>
            </v-row>
            <v-row class="grey darken-4 ma-0 pt-16 pb-16 pr-lg-12 pl-lg-12">
                <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pr-lg-5 pt-5 pb-16 pb-lg-5">
                    <v-timeline dense>
                        <v-timeline-item medium class="d-flex align-center" color="#21618C">
                            <div>
                                <span class="headline font-weight-bold font-color" color="white">EDUCATION</span>
                            </div>
                        </v-timeline-item>
                        <v-divider class="mb-5 ml-12" style="background: white"></v-divider>
                        <v-timeline-item
                            v-for="(education, i) in education"
                            :key="i"
                            :color="education.color"
                            small
                        >
                            <template>
                                <h3
                                    class="font-weight-medium font-color"
                                    v-text="education.title"
                                ></h3>
                            </template>
                            <div>
                                <span
                                    class="overline font-overline"
                                    v-text="education.year"
                                ></span>
                                <div class="font-color">
                                    {{ education.address }}
                                </div>
                            </div>
                        </v-timeline-item>
                    </v-timeline>
                </v-col>
                <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pl-lg-5 pt-16 pt-lg-5 pb-5">
                    <v-timeline dense>
                        <v-timeline-item medium class="d-flex align-center" color="#21618C">
                            <div>
                                <span class="headline font-weight-bold font-color">WORK EXPERIENCE</span>
                            </div>
                        </v-timeline-item>
                        <v-divider class="mb-5 ml-12" style="background: white"></v-divider>
                        <v-timeline-item
                            v-for="(experience, i) in experience"
                            :key="i"
                            :color="experience.color"
                            small
                        >
                            <template>
                                <h3
                                    class="font-weight-medium font-color"
                                    v-text="experience.title"
                                ></h3>
                            </template>
                            <div>
                                <span
                                    class="overline font-overline font-color"
                                    v-text="experience.year"
                                ></span>
                                <div class="font-color">
                                    {{ experience.address }}
                                </div>
                            </div>
                        </v-timeline-item>
                    </v-timeline>
                </v-col>
            </v-row>
        </v-main>
    </v-app>
</template>
<script>
  export default {
    data: () => ({
        education: [
            {
                color: '#3498DB',
                year: '2016 - 2020',
                title: 'Bachelor of Science in Information Technology',
                address: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut.'
            },
        ],
        experience: [
            {
                color: '#3498DB',
                year: '2021 - current',
                title: 'Position',
                address: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut.'
            },
            {
                color: '#3498DB',
                year: '2021 - current',
                title: 'Position',
                address: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut.'
            },
        ],
    }),
  }
</script>
<style scoped>
    .theme--light.v-timeline:before {
        background: white;
    }
    .font-color {
        color: #E0E0E0;
    }
    .font-overline {
        color: #E0E0E0;
        font-size: 16px !important;
    }
</style>
