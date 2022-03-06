<template>
  <div>
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-8">
      <a class="flex justify-center pt-8 sm:pt-0" href="https://nuxtjs.org" target="_blank">
        <svg width="218" height="45" viewBox="0 0 159 30" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M55.5017 6.81866H60.1727L70.0719 22.9912V6.81866H74.3837V29.7345H69.7446L59.8135 13.5955V29.7345H55.5017V6.81866Z" fill="#003543" /> <path d="M93.657 29.7344H89.6389V27.1747C88.7241 28.9761 86.8628 29.9904 84.5113 29.9904C80.7869 29.9904 78.3684 27.3059 78.3684 23.4423V13.2339H82.3865V22.5976C82.3865 24.8566 83.7594 26.4276 85.8171 26.4276C88.0712 26.4276 89.6389 24.6598 89.6389 22.2377V13.2339H93.657V29.7344Z" fill="#003543" /> <path d="M107.64 29.7344L103.784 24.2342L99.9291 29.7344H95.6492L101.596 21.1242L96.1074 13.2339H100.485L103.784 17.9821L107.051 13.2339H111.461L105.94 21.1242L111.886 29.7344H107.64Z" fill="#003543" /> <path d="M120.053 8.25848V13.2339H124.627V16.6063H120.053V24.7974C120.053 25.0725 120.162 25.3363 120.356 25.531C120.55 25.7257 120.813 25.8353 121.087 25.8357H124.627V29.728H121.98C118.386 29.728 116.035 27.6323 116.035 23.9687V16.6095H112.801V13.2339H114.83C115.776 13.2339 116.327 12.6692 116.327 11.7349V8.25848H120.053Z" fill="#003543" /> <path d="M134.756 24.5446V6.81866H139.066V23.1864C139.066 27.6067 136.943 29.7345 133.349 29.7345H128.332V25.8421H133.461C133.804 25.8421 134.134 25.7054 134.377 25.4621C134.619 25.2188 134.756 24.8888 134.756 24.5446Z" fill="#003543" /> <path d="M141.649 22.0409H145.799C146.029 24.6006 147.728 26.2308 150.472 26.2308C152.923 26.2308 154.623 25.2501 154.623 23.2199C154.623 18.3085 142.331 21.7129 142.331 12.9395C142.334 9.17515 145.568 6.55945 150.215 6.55945C155.05 6.55945 158.317 9.34153 158.516 13.6306H154.388C154.193 11.6341 152.632 10.2918 150.207 10.2918C147.953 10.2918 146.548 11.3397 146.548 12.9427C146.548 18.0173 159 14.2226 159 23.1576C159 27.4131 155.504 30 150.474 30C145.279 30 141.882 26.8563 141.654 22.0441" fill="#003543" /> <path d="M24.7203 29.704H41.1008C41.6211 29.7041 42.1322 29.5669 42.5828 29.3061C43.0334 29.0454 43.4075 28.6704 43.6675 28.2188C43.9275 27.7672 44.0643 27.2549 44.0641 26.7335C44.0639 26.2121 43.9266 25.6999 43.6662 25.2485L32.6655 6.15312C32.4055 5.70162 32.0315 5.32667 31.581 5.06598C31.1305 4.8053 30.6195 4.66805 30.0994 4.66805C29.5792 4.66805 29.0682 4.8053 28.6177 5.06598C28.1672 5.32667 27.7932 5.70162 27.5332 6.15312L24.7203 11.039L19.2208 1.48485C18.9606 1.03338 18.5864 0.658493 18.1358 0.397853C17.6852 0.137213 17.1741 0 16.6538 0C16.1336 0 15.6225 0.137213 15.1719 0.397853C14.7213 0.658493 14.3471 1.03338 14.0868 1.48485L0.397874 25.2485C0.137452 25.6999 0.000226653 26.2121 2.8053e-07 26.7335C-0.000226092 27.2549 0.136554 27.7672 0.396584 28.2188C0.656614 28.6704 1.03072 29.0454 1.48129 29.3061C1.93185 29.5669 2.44298 29.7041 2.96326 29.704H13.2456C17.3195 29.704 20.3239 27.9106 22.3912 24.4118L27.4102 15.7008L30.0986 11.039L38.1667 25.0422H27.4102L24.7203 29.704ZM13.0779 25.0374L5.9022 25.0358L16.6586 6.36589L22.0257 15.7008L18.4322 21.9401C17.0593 24.2103 15.4996 25.0374 13.0779 25.0374Z" fill="#00DC82" /></svg>
      </a>
      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
        <h2 class="text-2xl leading-7 font-semibold">
          Accounts
        </h2>
      </div>
    </div>
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-8">
      <div>
        <ul role="list" class="divide-y divide-gray-200">
          <li v-for="item in items.filter(i => i.accountType !== 'INVESTMENT')" :key="item.id">
            <div>
              <a href="#" class="block hover:bg-gray-50">
                <div class="px-4 py-4 sm:px-6">
                  <div class="flex items-center justify-between">
                    <div class="text-sm font-medium text-indigo-600 truncate">
                        {{item.name}}
                    </div>
                    <div class="ml-2 flex-shrink-0 flex">
                    <span class="px-2 inline-flex text-xs leading-5 font-semibold rounded-full bg-green-100 text-green-800">
                        Account No: {{item.accountNumber}}
                    </span>
                    </div>
                  </div>
                </div>
                <div class="mt-2 flex justify-between">
                    <div class="sm:flex">
                    <div class="mr-6 flex items-center text-sm text-gray-500">
                        <svg class="flex-shrink-0 mr-1.5 h-5 w-5 text-gray-400" x-description="Heroicon name: solid/users" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                            <path d="M9 6a3 3 0 11-6 0 3 3 0 016 0zM17 6a3 3 0 11-6 0 3 3 0 016 0zM12.93 17c.046-.327.07-.66.07-1a6.97 6.97 0 00-1.5-4.33A5 5 0 0119 16v1h-6.07zM6 11a5 5 0 015 5v1H1v-1a5 5 0 015-5z"></path>
                        </svg>
                        Account Type: {{item.accountType}}
                    </div>
                    </div>
                </div>
               <div class="mt-2 flex justify-between">
                    <div class="sm:flex">
                    <div class="mr-6 flex items-center text-sm text-gray-500">
                        Account Balance: {{item.balance | currency}}
                    </div>
                    </div>
                </div>                
                <div class="mt-2 flex justify-between">
                    <div class="sm:flex">
                    <hr/>
                    <div class="mr-6 flex items-center text-sm text-gray-500">
                        Transfer To: 
                    </div>
                    <select v-model="toAccount" class="block appearance-none w-full bg-gray-200 border border-gray-200 text-gray-700 py-3 px-4 pr-8 rounded leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-state">
                      <option v-for="toAcc in items.filter(i => i.id !== item.id)" :key="toAcc.id" v-bind:value="toAcc.accountNumber">{{toAcc.name}}</option>
                    </select>
                    <div class="mr-6 flex items-center text-sm text-gray-500">
                    <button @click="makeTransfer(item)" class="font-bold py-2 px-4 rounded bg-blue-500 text-white">
                      Confirm
                    </button>
                    </div>
                    </div>
                </div>
              </a>
            </div>
          </li>
        </ul>
      </div>
      <!-- <hr/>
      <div class="px-4 py-4 sm:px-6">
        <button class="font-bold py-2 px-4 rounded bg-blue-500 text-white">
          Create Account
        </button>
      </div> -->
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      toAccount: null,
      items: []
    }
  },
  methods: {
    makeTransfer(item: any) {
        var amount: any = window.prompt("Please enter amount to transfer: ");
        
        if (!amount) {
          window.alert("Invalid amount entered!")
          return;
        }
        amount = +amount;

        var transferRequest = {
          fromAccountId: item.id,
          toAccountNumber: this.toAccount,
          amount: amount
        };

        console.log(transferRequest);

        var myHeaders = new Headers();
        myHeaders.append("Accept", "application/json");
        myHeaders.append("Content-Type", "application/json");
        var requestOptions = {
          method: 'POST',
          headers: myHeaders,
          body: JSON.stringify(transferRequest)
        };

        fetch("http://localhost:8080/v1/accounts/transactions/", requestOptions)
        .then(response => response.json())
        .then(result => {
          console.log(result);
          this.$router.go(0);
        })
        .catch(error => console.log('error', error));

    }
  },
  created() {
    // watch the params of the route to fetch the data again
    this.$watch(
      () => this.$route.params,
      () => {
        const headers = { "Accept": "application/json" };

        var requestOptions = {
          method: 'GET',
          headers: headers
        };

        fetch("http://localhost:8080/v1/accounts/", requestOptions)
        .then(response => response.json())
        .then(result => {
          this.items = result;
          console.log(result);
        })
        .catch(error => console.log('error', error));
      },
      // fetch the data when the view is created and the data is
      // already being observed
      { immediate: true }
    )
  },
  name: 'AccountPage'
})
</script>
