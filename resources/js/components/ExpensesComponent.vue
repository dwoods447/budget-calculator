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
                <th><a href="javascript:void(0);" class="show" >Housing and Utilities</a></th>
                $<td><input name="monthly_income" type="text" v-model="rent_mortgage"></td>

            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" >Home or Renters Insurance</a></th>
                $<td><input name="monthly_income" type="text" v-model="home_renters_ins"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Property Tax</a></th>
                $<td><input name="monthly_income" type="text" v-model="prop_tax"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Condo or Homeowner Association (HOA) Fees</a></th>
                $<td><input  name="monthly_income" type="text" v-model="hoa_fees"></td>
            </tr>
            <tr class="header">
                <th><a href="" class="show">Total Monthly Expenses</a></th>
                $<td class><input id="total-monthly-expenses" name="total-monthly-expenses" type="text"  v-bind:value="getTotalExpenses"></td>
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
				home_renters_ins: 0,
                prop_tax: 0,
                hoa_fees: 0,
                total_expenses: 0,


            }
        },
        computed: {
             getTotalExpenses: function(){
				 this.total_expenses =  parseInt(this.rent_mortgage) + parseInt(this.home_renters_ins) + parseInt(this.prop_tax) + parseInt(this.hoa_fees);
				 //console.log('Monthly Income: '+ (this.monthly_income) + ' Total Income: '+ (this.other_income)+ ' = '  + this.total_income);
             	return this.total_expenses;
             }
        }
    }
</script>
