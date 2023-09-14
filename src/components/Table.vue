<script>
import ThreeDotIcon from './icons/ThreeDotIcon.vue';

export default {
    data() {
        return {
            desserts: [
                {
                    id: 1,
                    date: "17/05/22",
                    name: 'Amit Jain',
                    contact: "9753620608 amit@gmail.com",
                    refferedBy: "Sujay",
                    source: "IVR Call",
                },
                {
                    id: 2,
                    date: "17/05/22",
                    name: 'Amit Jain',
                    contact: "9753620608 amit@gmail.com",
                    refferedBy: "Sujay",
                    source: "IVR Call",
                },
                {
                    id: 3,
                    date: "17/05/22",
                    name: 'Amit Jain',
                    contact: "9753620608 amit@gmail.com",
                    refferedBy: "Sujay",
                    source: "IVR Call",
                },
                {
                    id: 4,
                    date: "17/05/22",
                    name: 'Amit Jain',
                    contact: "9753620608 amit@gmail.com",
                    refferedBy: "Sujay",
                    source: "IVR Call",
                },
                {
                    id: 5,
                    date: "17/05/22",
                    name: 'Amit Jain',
                    contact: "9753620608 amit@gmail.com",
                    refferedBy: "Sujay",
                    source: "IVR Call",
                },
                {
                    id: 5,
                    date: "17/05/22",
                    name: 'Amit Jain',
                    contact: "9753620608 amit@gmail.com",
                    refferedBy: "Sujay",
                    source: "IVR Call",
                },
                {
                    id: 6,
                    date: "17/05/22",
                    name: 'Amit Jain',
                    contact: "9753620608 amit@gmail.com",
                    refferedBy: "Sujay",
                    source: "IVR Call",
                },
            ],
        };
    },
    components: { ThreeDotIcon }
}
</script>
<template>
    <v-table class="mt-10">
        <thead>
            <tr>
                <th class="text-center">
                    Registration Date
                </th>
                <th class="text-center">
                    Client Name
                </th>
                <th class="text-center">
                    Contact
                </th>
                <th class="text-center">
                    Referred By
                </th>
                <th class="text-center">
                    Source
                </th>
                <th class="text-center">
                    Action
                </th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="item in desserts" :key="item.name">
                <td class="text-center">{{ item.date }}</td>
                <td class="text-center">{{ item.name }}</td>
                <td class="text-center">{{ item.contact }}</td>
                <td class="text-center">{{ item.refferedBy }}</td>
                <td class="text-center">{{ item.source }}</td>
                <td>
                    <v-btn class="tabelBtn" variant="outlined">
                        Edit
                    </v-btn>
                    <v-btn class="mx-2 tabelBtn" variant="outlined">
                        Delete
                    </v-btn>
                    <v-btn class="tabelBtn" variant="outlined">
                        <ThreeDotIcon/>
                    </v-btn>
                </td>
            </tr>
        </tbody>
    </v-table>
</template>

<style scoped>
th{
    color: #333 !important;
text-align: center;
font-family: Inter;
font-size: 12px !important;
font-style: normal;
font-weight: 600 !important;
line-height: 150%; /* 18px */
background:rgb(230, 229, 229);
}
td{
    color: #333;
text-align: center;
font-family: Inter;
font-size: 14px;
font-style: normal;
font-weight: 400;
line-height: 150%; /* 21px */
}
.tabelBtn{
    border-radius: 5px;
border: 1px solid #9D9D9D;
color: #9D9D9D;
text-align: center;
font-family: Inter;
font-size: 14px;
font-style: normal;
font-weight: 500;
line-height: 24px; /* 171.429% */
letter-spacing: -0.14px;
}
thead{
background-color:rgba(255, 255, 255, 0.5) !important;

}
</style>