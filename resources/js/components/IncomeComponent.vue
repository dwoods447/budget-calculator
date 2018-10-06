<template>
    <div class="income-container">


        <table>
            <thead>
            <tr>
                <th colspan="2">Enter Your Monthly Income</th>
            </tr>
            </thead>
            <tbody>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" id="take-home">Net Monthly Pay</a></th>
                $<td><input id="monthly_income" name="monthly_income" type="text" v-model="monthly_income"></td>
            </tr>
            <tr class="header">
                <th><a href="" class="show" id="other-income">Other Monthly Income</a></th>
                $<td class><input id="other_income" name="other_income" type="text"  v-model="other_income"></td>
            </tr>
            <tr class="header">
                <th><a href="" class="show" id="total-monthly-income">Total Monthly Income</a></th>
                $<td class><input id="total_monthly_income" name="total_monthly_income" type="text"  v-bind:value="getTotalMonthlyIncome"></td>

            </tr>

            <tr class="header">
                <th><a href="" class="show" id="total-yearly-income">Total Yearly Income</a></th>
                $<td class><input id="total_yearly_income" name="total_yearly_income" type="text"  v-bind:value="getTotalYearlyIncome"></td>
            </tr>
            </tbody>
        </table>
    </div>
</template>
<script>
    export default {
          data: function(){

              return{
                  other_income: 0,
                  monthly_income: 0,
                  total_income: 0,
                  yearly_income: 0,
              }

          },

         computed: {
              getTotalMonthlyIncome: function(){
                  this.total_income =  parseInt(this.other_income) + parseInt(this.monthly_income);
                  console.log('Monthly Income: '+ (this.monthly_income) + ' Total Income: '+ (this.other_income)+ ' = '  + this.total_income);
                 return this.total_income;
              },


              getTotalYearlyIncome: function(){
                  this.yearly_income =  (parseInt(this.other_income) + parseInt(this.monthly_income))  * parseInt(12);
                  return this.yearly_income;
              }
         }
    }
</script>