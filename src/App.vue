<template>
  <Header />
  <div class="container">
    <Balance />
    <IncomeExpense />
    <Transaction :transactions="transactions" />
    <AddTransaction />
  </div>
</template>

<script setup>
import Header from "./components/Header.vue";
import Balance from "./components/Balance.vue";
import IncomeExpense from "./components/IncomeExpense.vue";
import Transaction from "./components/Transaction.vue";
import AddTransaction from "./components/AddTransaction.vue";

import { ref } from "vue";
const transactions = ref([
  { id: 1, text: "Flower", amount: -19.99 },
  { id: 2, text: "Salary", amount: 299.97 },
  { id: 3, text: "Book", amount: -10 },
  { id: 4, text: "Camera", amount: 150 },
]);
</script>
