<template>
  <div class="bg-blue-700 mx-auto w-full pt-10">
    <div class="max-w-[350px] w-[350px] max-h-[220px] h-[220px] bg-black rounded-xl mx-auto px-[18px] py-[26px]">
      <div class="flex items-start justify-between">
        <h4 class="text-xs font-medium text-white">Credit Card</h4>
        <div>
          <svg width="50" height="31" viewBox="0 0 50 31" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M18.0532 27.1041H31.4354V3.24438H18.0532V27.1041Z" fill="#FF5F00"/>
          <path fill-rule="evenodd" clip-rule="evenodd" d="M18.903 15.1742C18.903 10.3336 21.1873 6.02247 24.7444 3.24432C22.1428 1.21225 18.8606 0 15.2928 0C6.8468 0 0.000244141 6.79382 0.000244141 15.1742C0.000244141 23.5545 6.8468 30.3484 15.2928 30.3484C18.8606 30.3484 22.1428 29.1361 24.7444 27.104C21.1873 24.3255 18.903 20.0147 18.903 15.1742Z" fill="#EB001B"/>
          <path fill-rule="evenodd" clip-rule="evenodd" d="M49.0111 24.577V23.9882H48.856L48.678 24.3932L48.4996 23.9882H48.3445V24.577H48.4537V24.1327L48.6211 24.5159H48.7345L48.9019 24.1319V24.577H49.0111ZM48.0293 24.577V24.0885H48.2281V23.989H47.7226V24.0885H47.921V24.577H48.0293ZM49.4886 15.1741C49.4886 23.5544 42.6416 30.3482 34.196 30.3482C30.6283 30.3482 27.3456 29.136 24.7444 27.1039C28.3015 24.3258 30.5858 20.0146 30.5858 15.1741C30.5858 10.3339 28.3015 6.02276 24.7444 3.2442C27.3456 1.21213 30.6283 -0.00012207 34.196 -0.00012207C42.6416 -0.00012207 49.4886 6.7937 49.4886 15.1741Z" fill="#F79E1B"/>
          </svg>
        </div>
      </div>
      <h1 class="text-xl text-white font-semibold mt-11">{{ cardNumber }}</h1>
      <div class="flex items-center justify-between text-white mt-14">
        <p class="text-xs font-medium">{{ cardName }}</p>
        <p class="text-xs font-medium">{{ cardTerm }}</p>
      </div>
    </div>
    <div class="w-[350px] h-[220px] mx-auto bg-white rounded-xl space-y-10 mt-10 px-[18px] py-[26px]">
      <input class="w-full outline-none border border-black rounded-md px-2 py-1" type="number" v-model="cardNumber" placeholder="Card Number">
      <input class="w-full outline-none border border-black rounded-md px-2 py-1" type="text" v-model="cardName" placeholder="Card Name">
      <input class="w-full outline-none border border-black rounded-md px-2 py-1" type="Number" v-model="cardTerm" placeholder="Card Term">
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        cardNumber: '',
        cardName: '',
        cardTerm: ''
      }
    },
    methods: {
      // insertData(val) {
      //   this.cardNumber = val
      // }
    },
  }
</script>


<style scoped>
  
</style>
