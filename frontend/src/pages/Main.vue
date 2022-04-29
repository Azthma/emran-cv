<template>
    <v-app>
        <v-main>
            <v-row class="grey darken-3 pt-16 pb-16" no-gutters>
                <v-col cols="12" md="6" class="d-flex justify-center justify-lg-end align-center pr-lg-12 pt-5 pb-5">
                    <v-avatar size="200">
                        <img 
                            style="object-fit: cover;"
                            src="../assets/profile.png"
                        >
                    </v-avatar>
                </v-col>
                <v-col cols="12" md="6" class="d-flex justify-center justify-lg-start align-center pl-lg-12 pt-5 pb-5">
                    <v-row>
                        <v-col cols="12" class="d-flex justify-center justify-lg-start align-center pb-0 font-color">
                            <h1>Emran Pendaliday</h1>
                        </v-col>
                        <v-col cols="12" class="d-flex justify-center justify-lg-start align-center pt-0 font-color">
                            <h2>Web Developer, Quality Assurance</h2>
                        </v-col>
                        <v-col cols="12" class="d-flex justify-center justify-lg-start align-center pt-0 font-color">
                            <v-btn class="mt-5" outlined rounded color="white">Download</v-btn>
                        </v-col>
                    </v-row>
                </v-col>
            </v-row>
            <v-card flat>
                <v-tabs
                    v-model="tab"
                    background-color="grey darken-4"
                    centered
                    dark
                    icons-and-text
                >
                    <v-tabs-slider></v-tabs-slider>
                    <v-tab href="#about">
                        <v-icon>mdi-account</v-icon>
                    </v-tab>
                    <v-tab href="#background">
                        <v-icon>mdi-draw-pen</v-icon>
                    </v-tab>
                    <v-tab href="#skills">
                        <v-icon>mdi-briefcase</v-icon>
                    </v-tab>
                    <v-tab href="#contact">
                        <v-icon>mdi-phone</v-icon>
                    </v-tab>
                </v-tabs>
                <v-tabs-items v-model="tab">
                    <v-tab-item
                        :value="'about'"
                    >
                        <About />
                    </v-tab-item>
                </v-tabs-items>
                <v-tabs-items v-model="tab">
                    <v-tab-item
                        :value="'skills'"
                    >
                        <Skills />
                    </v-tab-item>
                </v-tabs-items>
                <v-tabs-items v-model="tab">
                    <v-tab-item
                        :value="'background'"
                    >
                        <Background />
                    </v-tab-item>
                </v-tabs-items>
                <v-tabs-items v-model="tab">
                    <v-tab-item
                        :value="'contact'"
                    >
                        <Contact />
                    </v-tab-item>
                </v-tabs-items>
            </v-card>
        </v-main>
    </v-app>
</template>
<script>
import About from "../components/About.vue";
import Background from "../components/Background.vue";
import Skills from "../components/Skills.vue";
import Contact from "../components/Contact.vue";
export default {
    components: {
        Background,
        Skills,
        About,
        Contact,
    },
    data: () => ({
        tab: null,
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
