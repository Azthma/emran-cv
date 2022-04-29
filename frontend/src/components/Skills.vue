<template>
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
                <v-list class="grey darken-4" dense>
                    <v-list-item
                        v-for="(soft_skills, i) in soft_skills"
                        :key="i"
                    >
                        <v-list-item-icon class="mr-3">
                            <v-icon
                                color="green"
                            >
                                mdi-check
                            </v-icon>
                        </v-list-item-icon>
                        <v-list-item-content>
                            <v-list-item-title class="font-color">
                                <span
                                    class="overline font-overline"
                                    v-text="soft_skills.name"
                                ></span>
                            </v-list-item-title>
                        </v-list-item-content>
                    </v-list-item>
                </v-list>
            </v-card>
        </v-col>
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
                        <h3 class="font-weight-bold font-color">HARD SKILLS</h3>
                    </v-chip>
                </v-layout>
                <v-list class="grey darken-4" dense>
                    <v-list-item
                        v-for="(hard_skills, i) in hard_skills"
                        :key="i"
                    >
                        <v-list-item-icon class="mr-3">
                            <v-icon
                                color="green"
                            >
                                mdi-check
                            </v-icon>
                        </v-list-item-icon>

                        <v-list-item-content class="pb-0">
                            <v-list-item-title v-if="hard_skills.skills" class="font-color">
                                <span
                                    class="overline font-overline"
                                    v-text="hard_skills.name"
                                ></span>
                            </v-list-item-title>
                            <v-list-item-title v-else class="font-color">
                                <span
                                    class="overline font-overline"
                                    v-text="hard_skills.name"
                                ></span>
                            </v-list-item-title>
                            <v-list v-if="hard_skills.skills" class="grey darken-4 py-0" dense>
                                <v-list-item
                                    v-for="(skill, i) in hard_skills.skills"
                                    :key="i"
                                >
                                    <v-list-item-icon class="mr-3">
                                        <v-icon
                                            color="green"
                                        >
                                            mdi-check
                                        </v-icon>
                                    </v-list-item-icon>
                                    <v-list-item-content>
                                        <v-list-item-title class="font-color">
                                            <span
                                                class="overline font-overline"
                                                v-text="skill.name"
                                            ></span>
                                        </v-list-item-title>
                                    </v-list-item-content>
                                </v-list-item>
                            </v-list>
                        </v-list-item-content>
                    </v-list-item>
                </v-list>
            </v-card>
        </v-col>
        <v-col cols="12" md="4" class="d-flex justify-lg-start pr-lg-5 pt-5 pb-16 pb-lg-5">
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
</template>
<script>
  export default {
    data: () => ({
        soft_skills: [
            {
                name: "Critical Thinking"
            },
            {
                name: "Problem-solving"
            },
            {
                name: "Time and project management"
            },
            {
                name: "Teamwork"
            },
            {
                name: "Adaptability"
            }
        ],
        hard_skills: [
            {
                name: "Front-end Frameworks",
                skills: [
                    {name: "VueJs"},
                    {name: "React"},
                    {name: "Bootstrap"},
                ]
            },
            {
                name: "Back-end Frameworks",
                skills: [
                    {name: "Express"},
                ]
            },
            {
                name: "Unit Testing Frameworks",
                skills: [
                    {name: "Mocha And Chai"},
                    {name: "Selenium"},
                    {name: "Phpunit"},
                ]
            },
            {
                name: "NodeJs",
            },
            {
                name: "Sequelize",
            },
            {
                name: "Git",
            }
        ],
        programming_language: [
            {
                name: "Javascript",
                value: 90
            },
            {
                name: "PHP",
                value: 85
            },
            {
                name: "HTML",
                value: 85
            },
            {
                name: "CSS",
                value: 90
            },
            {
                name: "C#",
                value: 75
            },
            {
                name: "Visual Basic",
                value: 75
            },
            {
                name: "SQL",
                value: 90
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
</style>