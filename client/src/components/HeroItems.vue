<template>
    <div>
        <v-toolbar-items>
            <v-layout justify-center align-end mt-7 ml-10>
                <v-layout justify-center align-end white--text>

                    <img src="../assets/building_health_healthcare_hospital_medic_medical_icon_127271.png"
                         alt="hospital">
                    <v-toolbar-title class="ml-3 line text-h5 font-weight-bold text-uppercase">
                        mayo clinic</v-toolbar-title>

                    <!--menuComp-->
                    <v-menu bottom left>
                        <template v-slot:activator="{ on, attrs }">
                            <v-toolbar-title
                                icon
                                v-bind="attrs"
                                v-on="on"
                                class="ml-10">
                                患者様へ ▼
                            </v-toolbar-title>
                        </template>

                        <v-list>
                            <v-list-item
                                v-for="(item, i) in items"
                                :key="i"
                                @click="i"
                            >
                                <v-list-item-title>{{ item.title }}</v-list-item-title>
                            </v-list-item>
                        </v-list>
                    </v-menu>
                    <!--/menuComp-->

                    <v-toolbar-title class="ml-10">医療関係者の方へ</v-toolbar-title>
                </v-layout>
            </v-layout>
            <v-spacer></v-spacer>
            <v-layout justify-center align-end mt-7>
                <v-toolbar-title>4</v-toolbar-title>
                <v-toolbar-title>5</v-toolbar-title>
            </v-layout>
        </v-toolbar-items>
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [
                { title: '院内の案内' },
                { title: '院内の案内' },
                { title: '院内の案内' },
                { title: '院内の案内' }
            ]
        };
    },
    methods: {
        log() {
            console.log('aaa');
        }
    }
};

</script>
