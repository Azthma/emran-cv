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
                    <v-timeline dense class="pt-0">
                        <v-timeline-item large class="d-flex align-center" color="#21618C">
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
                    <v-timeline dense class="pt-0">
                        <v-timeline-item large class="d-flex align-center" color="#21618C">
                            <template v-slot:icon>
                                <v-icon color="white">
                                    mdi-briefcase
                                </v-icon>
                            </template>
                            <div>
                                <span class="headline font-weight-bold font-color">WORK EXPERIENCE</span>
                            </div>
                        </v-timeline-item>
                        <v-divider class="mb-5 ml-12" style="background: white"></v-divider>
                        <v-timeline-item
                            v-for="(experience, i) in experience"
                            :key="i"
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
            <v-divider style="background-color:'white';"></v-divider>
            <v-row class="grey darken-4 ma-0 pt-16 pb-16 pr-lg-12 pl-lg-12">
                <v-col cols="12" md="4" class="d-flex justify-lg-start pr-lg-5 pt-5 pb-16 pb-lg-5">
                    <v-card
                        class="grey darken-4"
                        flat
                    >
                        <v-layout>
                            <v-chip
                                class="pa-4"
                                color="white"
                                outlined
                            >
                                <h3 class="font-weight-bold font-color">SOFT SKILLS</h3>
                            </v-chip>
                        </v-layout>
                        <v-timeline dense>
                            <v-timeline-item
                                v-for="(soft_skills, i) in soft_skills"
                                :key="i"
                                small
                            >
                                <template>
                                    <h3
                                        class="font-weight-medium font-color"
                                        v-text="soft_skills.name"
                                    ></h3>
                                </template>
                            </v-timeline-item>
                        </v-timeline>
                    </v-card>
                </v-col>
                <v-col cols="12" md="4" class="d-flex justify-lg-start pl-lg-5 pt-16 pt-lg-5 pb-5">
                    <v-card
                        class="grey darken-4"
                        flat
                    >
                        <v-layout>
                            <v-chip
                                class="pa-4"
                                color="white"
                                outlined
                            >
                                <h3 class="font-weight-bold font-color">HARD SKILLS</h3>
                            </v-chip>
                        </v-layout>
                        <v-timeline dense align-top>
                            <v-timeline-item
                                v-for="(hard_skills, i) in hard_skills"
                                :key="i"
                                small
                            >
                                <template>
                                    <h3
                                        class="font-weight-medium font-color mb-2"
                                        v-text="hard_skills.name"
                                    ></h3>
                                    <v-timeline v-if="hard_skills.skills" dense>
                                        <v-timeline-item
                                            v-for="(skill, i) in hard_skills.skills"
                                            :key="i"
                                            small
                                        >
                                            <template>
                                                <h3
                                                    class="font-weight-medium font-color"
                                                    v-text="skill.name"
                                                ></h3>
                                            </template>
                                        </v-timeline-item>
                                    </v-timeline>
                                </template>
                            </v-timeline-item>
                        </v-timeline>
                    </v-card>
                </v-col>
                <v-col cols="12" md="4" class="d-flex justify-center justify-lg-start pl-lg-5 pt-16 pt-lg-5 pb-5">
                    <v-col>
                        <v-chip
                            class="pa-4 mb-3"
                            color="white"
                            outlined
                        >
                            <h3 class="font-weight-bold font-color">PROGRAMMING LANGUAGE</h3>
                        </v-chip>
                        <v-list-item two-line v-for="(programming_language, i) in programming_language" :key="i">
                            <v-list-item-content>
                                <v-list-item-title class="font-color mb-2"><strong>{{programming_language.name}}</strong></v-list-item-title>
                                <v-progress-linear
                                    color="blue"
                                    rounded
                                    height="10"
                                    :value="programming_language.value"
                                ></v-progress-linear>
                            </v-list-item-content>
                        </v-list-item>
                    </v-col>
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
                year: '2016 - 2020',
                title: 'Bachelor of Science in Information Technology',
                address: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut.'
            },
        ],
        experience: [
            {
                year: '2021 - current',
                title: 'Position',
                address: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut.'
            },
            {
                year: '2021 - current',
                title: 'Position',
                address: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut.'
            },
        ],
        soft_skills: [
            {
                name: "Neque porro"
            },
            {
                name: "Neque porro"
            },
            {
                name: "Neque porro"
            },
            {
                name: "Neque porro"
            },
            {
                name: "Neque porro"
            }
        ],
        hard_skills: [
            {
                name: "Neque porro",
                skills: [
                    {name: "one dsa da"},
                    {name: "two"},
                ]
            },
            {
                name: "Neque porro",
                skills: [
                    {name: "twodasd sda"},
                ]
            },
            {
                name: "Neque porro",
            },
            {
                name: "Neque porro",
            }
        ],
        programming_language: [
            {
                name: "N321321321",
                value: 80
            },
            {
                name: "asdsadasdsa",
                value: 85
            }
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
