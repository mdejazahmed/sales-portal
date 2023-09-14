<script setup>
import Table from '@/components/Table.vue';
import DownArrowIcon from '../components/icons/DownArrowIcon.vue';
import SearchIcon from '../components/icons/SearchIcon.vue';
import DialogBtn from '@/components/DialogBtn.vue';

</script>

<template>
  <div class="leads">
    <!-- filters -->
    <div class="shortingContainer">
      <div class="searchContainer">
        <SearchIcon />
        <input type="search" placeholder="Search name, email, or etc.">
      </div>
      <div class="filterContainer">
        <p>Filter by source</p>
        <DownArrowIcon />
      </div>
     <DialogBtn class="dialogBtn"/>
    </div>
    <!-- filters -->

    <Table/>
    
  </div>
</template>

<style scoped>
.dialogBtn{
  margin-left: auto;
  margin-right: 27px;
}
.leads {
  width: 100%;
  min-height: 100vh;
  background: #ECECEC;
  padding-top: 16px;
}

.shortingContainer {
  display: flex;
  gap: 25.65px;
}

.searchContainer {
  display: flex;
  width: 313.223px;
  height: 40px;
  padding: 9px 8px;
  align-items: center;
  gap: 8px;
  border-radius: 5px;
  background: #FFF;
  margin-left: 16px;
}

input {
  width: 100%;
}

.filterContainer {
  width: 207.433px;
  height: 40px;
  flex-shrink: 0;
  border-radius: 5px;
  background: #FFF;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 17px 0 22px;
  color: #333333d4;
font-family: Inter;
font-size: 14px;
font-style: normal;
font-weight: 400;
line-height: 24px; /* 171.429% */
}

.addBtn{
  border-radius: 5px;
background: #3C91F4;
width: 102px;
height: 40px;
color: #FFF;
text-align: center;
font-family: Inter;
font-size: 14px;
font-style: normal;
font-weight: 500;
line-height: 24px; /* 171.429% */
letter-spacing: -0.14px;
margin-left: auto;
margin-right: 27px;
}

table {
  width: 100%;
  margin-top: 50px;
  border: none;
}

thead {
  background: rgba(255, 255, 255, 0.5);
  height: 62px;
}

tbody {
  border-top: 1px solid rgba(51, 51, 51, 0.10);
  background: #FFF;
}

tbody tr {
  height: 72px;
}

td {
  text-align: center;
}
td button{
  border-radius: 5px;
border: 1px solid #9D9D9D;
background: transparent;
color: #9D9D9D;
text-align: center;
font-family: Inter;
font-size: 14px;
font-style: normal;
font-weight: 500;
line-height: 24px; /* 171.429% */
letter-spacing: -0.14px;
padding: 3px 10px;
margin:0 5px ;
}
</style>