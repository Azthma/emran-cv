<template>
    <div>
        <v-row class="grey darken-4 ma-0 pt-16 pb-16 pr-lg-12 pl-lg-12">
            <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start pr-lg-5 pt-5 pb-16 pb-lg-5">
                <v-timeline align-top dense class="pt-0">
                    <v-timeline-item large class="d-flex align-center" color="#212121">
                        <template v-slot:icon>
                            <v-icon color="white">
                                mdi-school
                            </v-icon>
                        </template>
                        <div>
                            <span class="headline font-weight-bold font-color" color="white">EDUCATION</span>
                        </div>
                    </v-timeline-item>
                    <v-divider class="mb-5 ml-12" style="background: white"></v-divider>
                    <v-timeline-item
                        v-for="(education, i) in education"
                        :key="i"
                        small
                        color="#212121"
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
                <v-timeline align-top dense class="pt-0">
                    <v-timeline-item large class="d-flex align-center" color="#212121">
                        <template v-slot:icon>
                            <v-icon color="white">
                                mdi-briefcase
                            </v-icon>
                        </template>
                        <div>
                            <span class="headline font-weight-bold font-color">EXPERIENCE</span>
                        </div>
                    </v-timeline-item>
                    <v-divider class="mb-5 ml-12" style="background: white"></v-divider>
                    <v-timeline-item
                        v-for="(experience, i) in experience"
                        :key="i"
                        small
                        color="#212121"
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
        <v-divider></v-divider>
        <v-row class="grey darken-4 ma-0 pt-16 pb-16 pr-lg-12 pl-lg-12">
            <v-col cols="12" md="6" class="d-flex justify-lg-start pl-5 pt-5 pb-16 pb-lg-5">
                <v-col>
                    <v-row>
                        <v-avatar color="#212121" style="border: 4px solid white">
                            <v-icon dark>
                                mdi-certificate
                            </v-icon>
                        </v-avatar>
                        <div class=" d-flex align-center ml-5">
                            <span class="headline font-weight-bold font-color" color="white">CERTIFICATE</span>
                        </div>
                    </v-row>
                    <v-col class="mt-9 pl-0">
                        <v-card
                            outlined
                        >
                                    <v-list-item three-line>
                                        <v-list-item-content>
                                            <h2 class="text-h5">
                                                Devfest Zamboanga Peninsula 2018: Machine Learning, Android, Cyber Security, Flutter, Google Cloud, Python and Emerging Tools
                                            </h2>
                                            <div class="text-overline">
                                                Google Developers Group - December 4, 2018
                                            </div>
                                            <v-list-item-subtitle>Social Hall, College of Teacher Education, Western Mindanao State University</v-list-item-subtitle>
                                        </v-list-item-content>
                                    </v-list-item>
                        </v-card>
                    </v-col>
                </v-col>
            </v-col>
        </v-row>
    </div>
</template>
<script>
  export default {
    data: () => ({
        education: [
            {
                year: '2016 - 2020',
                title: 'Bachelor of Science in Information Technology',
                address: 'Normal Road, Baliwasan, Zamboanga City'
            },
        ],
        experience: [
            {
                year: '2021 - current',
                title: 'Quality Assurance - SECRET',
                address: 'Minglanilla City, Cebu, Philippines'
            },
            {
                year: '486 Hours',
                title: 'IT Support - OJT',
                address: 'A&S Building Suterville, San Jose Gusu, Zamboanga City, 7000'
            },
        ]
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