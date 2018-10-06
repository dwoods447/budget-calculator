<template>
    <div class="expense-container">
        <table>
            <thead>
            <tr>
                <th>Enter Your Monthly Expenses</th>
            </tr>
            </thead>

            <tbody>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" id="">Housing and Utilities</a></th>
                $<td><input id="" name="monthly_income" type="text" v-model="rent_mortgage"></td>

            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" id="">Home or Renters Insurance</a></th>
                $<td><input id="" name="monthly_income" type="text" v-model="monthly_income"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" id="">Property Tax</a></th>
                $<td><input id="" name="monthly_income" type="text" v-model="monthly_income"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" id="take-home">Condo or Homeowner Association (HOA) Fees</a></th>
                $<td><input id="" name="monthly_income" type="text" v-model="monthly_income"></td>
            </tr>
            </tbody>
        </table>
    </div>
</template>

<script>

    export default {
        data: function(){
            return {
                rent_mortgage: 0,
            }
        },
        computed: {

        }
    }
</script>
