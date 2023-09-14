<template>
  <div class="text-center">
    <v-btn class="addLeadsBtn" color="primary" @click="dialog = true">
      + Add Leads
    </v-btn>

    <v-dialog v-model="dialog" width="auto">
      <div class="dialogCard">
        <div class="cardHeader">
          <div class="text">
            <h2>Add Lead</h2>
            <p>Please enter details here</p>
          </div>
          <button class="closeBtn" @click="dialog = false">x</button>
        </div>
        <form>
          <div class="splitDiv">
            <v-text-field
            class="input"
            label="First Name"
            variant="outlined"
          ></v-text-field>
            <v-text-field
            label="Last Name"
            variant="outlined"
          ></v-text-field>
          </div>
          <v-text-field
            label="Mobile Number"
            variant="outlined"
          ></v-text-field>
          <v-text-field
            label="Email"
            variant="outlined"
          ></v-text-field>
          <v-select
  label="Select"
  :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
  variant="outlined"
></v-select>
          <v-select
  label="Select"
  :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
  variant="outlined"
></v-select>
          <v-select
  label="Select"
  :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
  variant="outlined"
></v-select>
          <v-select
  label="Select"
  :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
  variant="outlined"
></v-select>
<v-textarea label="Label" variant="outlined"></v-textarea>
<button class="saveBtn" @click="dialog=false">Save</button>
        </form>
      </div>
    </v-dialog>
  </div>
</template>

<script >

export default {
  data() {
    return {
      dialog: false,
    }
  },
}
</script>

<style scoped>
.saveBtn{
  width: 165.143px;
height: 40px;
border-radius: 5px;
background: #3C91F4;
color: #FFF;
text-align: center;
font-family: Inter;
font-size: 16px;
font-style: normal;
font-weight: 500;
line-height: 24px; /* 150% */
letter-spacing: -0.16px;
margin-bottom: 30vh;
display: block;
margin-left: auto;
}
.input{
  height: 46px;
  border-radius: 3.5px;
border-color: #6200EE;
}
.splitDiv{
  display: flex;
  justify-content: space-between;
  gap: 14px;
}
form{
  width: 100%;
  padding: 27px 39px;
  height: calc(719px - 91px);
  overflow-x: scroll;
}
.closeBtn {
  width: 24px;
  height: 24px;
  border-radius: 50%;
  background: white !important;
  color: #3C91F4 !important;
  display: flex;
  align-items: center;
  justify-content: center;
}
.text h2 {
  color: #FFF;
  font-family: Inter;
  font-size: 24px;
  font-style: normal;
  font-weight: 600;
  line-height: 24px;
  /* 100% */
  letter-spacing: -0.24px;
}

.text p {
  color: #FFF;
  font-family: Inter;
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: 14px;
  /* 116.667% */
  letter-spacing: -0.12px;
}


.cardHeader {

  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 91px;
  background: #3C91F4;
  box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.25);
  padding: 0 39px;
}

.dialogCard {
  width: 665px;
  height: 719px;
  background-color: white;
  border-radius: 20px;
  overflow: hidden;

}

.addLeadsBtn {
  border-radius: 5px;
  background: #3C91F4;
  color: #FFF;
  text-align: center;
  font-family: Inter;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;
  /* 171.429% */
  letter-spacing: -0.14px;
}</style>