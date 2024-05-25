<template>
  <Header />
  <div class="container">
    <Balance />
    <IncomeExpense />
    <Transaction />
    <AddTransaction />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Balance from "./components/Balance.vue";
import IncomeExpense from "./components/IncomeExpense.vue";
import Transaction from "./components/Transaction.vue";
import AddTransaction from "./components/AddTransaction.vue";

export default {
  components: {
    Header,
    Balance,
    IncomeExpense,
    Transaction,
    AddTransaction,
  },
};
</script>
