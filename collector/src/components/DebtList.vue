<template>
    <ul>
        <li v-for="(debt, id) in debts" :key="id" >
            {{debt.name}} by {{ debt.who }}
            {{debt.amount}}
        </li>
    </ul>
</template>

<script>
import Debt from './Debt'

export default {
    name: 'DebtList',
    components: {
      Debt
    },
    props: ['debts'],
}
</script>

<style>

</style>