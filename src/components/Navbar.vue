<template>
     <v-app-bar class="nav px-4">
               <div class="left">
                    <RouterLink to="/" class="logo">SALES PORTAL</RouterLink>
                    <p class="path">Client Management/ <span>Leads</span></p>
               </div>
               <v-spacer></v-spacer>
               <div class="right">
                    <div class="profile">AK</div>
                    <div class="name">A K Satish</div>
                    <DownArrowIcon />
               </div>
     </v-app-bar>
</template>

<style scoped>
.nav {
     background-color: red;
}

.left {
     display: flex;
     align-items: center;
     gap: 10px;
}

.logo {
     color: #3C91F4;
     font-family: Inter;
     font-size: 16px;
     font-style: normal;
     font-weight: 700;
     line-height: 48px;
     /* 300% */
}

.path {
     color: #333;
     font-family: Inter;
     font-size: 16px;
     font-style: normal;
     font-weight: 600;
     line-height: 48px;
     /* 300% */
}

.path span {
     color: #333;
     font-family: Inter;
     font-size: 16px;
     font-style: normal;
     font-weight: 400;
     line-height: 48px;
}

.right {
     display: flex;
     align-items: center;
     gap: 10px;
}

.profile {
     height: 41px;
     width: 41px;
     background-color: #333333c8;
     border-radius: 50%;
     display: flex;
     align-items: center;
     justify-content: center;
     color: #FFF;
     font-family: Source Sans Pro;
     font-size: 18px;
     font-style: normal;
     font-weight: 400;
     line-height: normal;
     letter-spacing: 2.16px;
}

.name {
     color: #333;
     font-family: Inter;
     font-size: 14px;
     font-style: normal;
     font-weight: 400;
     line-height: normal;
}
</style>