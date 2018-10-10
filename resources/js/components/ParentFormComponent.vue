<template>
    <div class="income-container">
        <table>
                <thead>
                <tr>
                    <th colspan="2"><span v-b-toggle.collapse1><i class="fas fa-chevron-down"></i></span>&nbsp;&nbsp;&nbsp;Enter Your Monthly Income</th>
                </tr>
                </thead>
                <tbody>
                <b-collapse id="collapse1" class="mt-2">
                <tr class="header">
                    <th><a href="javascript:void(0);" class="show" id="take-home">Net Monthly Pay</a></th>
                    $<td><input id="monthly_income" name="monthly_income" type="text" v-model="monthly_income"></td>
                </tr>
                <tr class="header">
                    <th><a href="javascript:void(0);" class="show" id="other-income">Other Monthly Income</a></th>
                    $<td class><input id="other_income" name="other_income" type="text"  v-model="other_income"></td>
                </tr>
                </b-collapse>
                </tbody>
       </table>

        <table>
            <thead>
            <tr>
                <th colspan="2">Enter Your Monthly Expenses</th>
            </tr>
            </thead>
            <tbody>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" >Rent of Mortgage</a></th>
                $<td><input  id="rent_mortgage" name="rent_mortgage" type="text" v-model="rent_mortgage"></td>

            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" >2nd Mortgage</a></th>
                $<td><input  id="second_mortgage" name="second_mortgage" type="text" v-model="second_mortgage"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show" >Home or Renters Insurance</a></th>
                $<td><input id="home_renters_ins" name="home_renters_ins" type="text" v-model="home_renters_ins"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Property Tax</a></th>
                $<td><input id="prop_tax" name="prop_tax" type="text" v-model="prop_tax"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Condo or Homeowner Association (HOA) Fees</a></th>
                $<td><input  id="hoa_fees" name="hoa_fees" type="text" v-model="hoa_fees"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">Home Repairs & Maintenance</a></th>
                $<td><input id="home_repair" name="home_repair" type="text"  v-model="home_repair"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Electric & Gas</a></th>
                $<td><input  id="electric_gas" name="electric_gas" type="text"  v-model="electric_gas"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">Water & Sewer</a></th>
                $<td><input id="water_sewer" name="water_sewer" type="text"  v-model="water_sewer"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Phone & Cell</a></th>
                $<td><input  id="phone_cell" name="phone_cell" type="text"  v-model="phone_cell"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">Cable & Internet</a></th>
                $<td><input id="cable_internet" name="cable_internet" type="text"  v-model="cable_internet"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Car Payment</a></th>
                $<td><input  id="car_payment" name="car_payment" type="text"  v-model="car_payment"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">2nd Car Payment</a></th>
                $<td><input id="second_car_payment" name="second_car_payment" type="text"  v-model="second_car_payment"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Monthly Car Insurance</a></th>
                $<td><input  id="car_insurance" name="car_insurance" type="text"  v-model="car_insurance"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">Gasoline</a></th>
                $<td><input id="gas" name="gas" type="text"  v-model="gas"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">Parking/Tolls</a></th>
                $<td><input id="parking_tolls" name="parking_tolls" type="text"  v-model="parking_tolls"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Groceries & Household Goods</a></th>
                $<td><input  id="groceries_household" name="groceries_household" type="text"  v-model="groceries_household"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">School Lunches</a></th>
                $<td><input id="school_lunch" name="school_lunch" type="text"  v-model="school_lunch"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Eating Out</a></th>
                $<td><input  id="eating_out" name="eating_out" type="text"  v-model="eating_out"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">Health Insurance & Co-pays </a></th>
                $<td><input id="health_ins_copay" name="health_ins_copay" type="text"  v-model="health_ins_copay"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Prescriptions</a></th>
                $<td><input  id="prescription" name="prescription" type="text"  v-model="prescription"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">Life Insurance </a></th>
                $<td><input id="life_ins" name="life_ins" type="text"  v-model="life_ins"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Clothing for Family</a></th>
                $<td><input  id="clothing" name="clothing"  type="text"  v-model="clothing"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">Dry Cleaning & Laundry</a></th>
                $<td><input id="dry_cleaning" name="dry_cleaning" type="text"  v-model="dry_cleaning"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Barber & Beauty Shop</a></th>
                $<td><input  id="barber_shop" name="barber_shop" type="text"  v-model="barber_shop"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">Child Care</a></th>
                $<td><input id="child_care" name="child_care" type="text"  v-model="child_care"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Child Support Payments</a></th>
                $<td><input  id="child_support" name="child_support" type="text"  v-model="child_support"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">School Tuition & Supplies</a></th>
                $<td><input id="school_supplies" name="school_supplies" type="text"  v-model="school_supplies"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Credit Cards </a></th>
                $<td><input id="credit_cards" name="credit_cards" type="text"  v-model="credit_cards"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">Retail Store Cards</a></th>
                $<td><input id="store_cards" name="store_cards" type="text"  v-model="store_cards"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Medical Debt </a></th>
                $<td><input id="medical_debt" name="medical_debt"  type="text"  v-model="medical_debt"></td>
            </tr>
            <tr>
                <th><a href="javascript:void(0);" class="show">Student Loans </a></th>
                $<td><input id="student_loans" name="student_loans" type="text"  v-model="student_loans"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Tax Payments</a></th>
                $<td><input  id="tax_payments" name="tax_payments" type="text"  v-model="tax_payments"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">Miscellaneous Debt Payments</a></th>
                $<td><input id="miscellaneous_debt_payments" name="miscellaneous_debt_payments" type="text"  v-model="miscellaneous_debt_payments"></td>
            </tr>



            <tr>
                <th><a href="javascript:void(0);" class="show">ATM Fees</a></th>
                $<td><input id="atm_fees" name="atm_fees" type="text"  v-model="atm_fees"></td>
            </tr>
            <tr>
                <th><a href="javascript:void(0);" class="show">Monthly Subscriptions</a></th>
                $<td><input id="monthly_subscriptions" name="monthly_subscriptions" type="text"  v-model="monthly_subscriptions"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Hobbies & Sports</a></th>
                $<td><input  id="hobbies_sports" name="hobbies_sports" type="text"  v-model="hobbies_sports"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Newspaper & Magazines</a></th>
                $<td><input id="news_magazines" name="news_magazines" type="text"  v-model="news_magazines"></td>
            </tr>

            <tr>
                <th><a href="javascript:void(0);" class="show">Travel & Recreation</a></th>
                $<td><input id="travel_recreation" name="travel_recreation" type="text"  v-model="travel_recreation"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Church & Charitable Donations</a></th>
                $<td><input id="church_charity"  name="church_charity" type="text"  v-model="church_charity"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">Pet Care</a></th>
                $<td><input id="pet_care" name="pet_care" type="text"  v-model="pet_care"></td>
            </tr>
            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Holidays & Birthdays </a></th>
                $<td><input  id="holiday_birthday" type="text"  v-model="holiday_birthday"></td>
            </tr>


            <tr>
                <th><a href="javascript:void(0);" class="show">Other Expenses</a></th>
                $<td><input id="other_expenses" name="other_expenses" type="text"  v-model="other_expenses"></td>
            </tr>

            <tr class="header">
                <th><a href="javascript:void(0);" class="show">Total Monthly Expenses</a></th>
                $<td><input id="total_monthly_expenses" name="total_monthly_expenses" type="text"  v-bind:value="getTotalExpenses"></td>
            </tr>


            <tr class="header">
                <th><a href="javascript:void(0);" class="show" id="total-monthly-income">Total Monthly Income</a></th>
                $<td class><input id="total_monthly_income" name="total_monthly_income" type="text"  v-bind:value="getTotalMonthlyIncome"></td>
            </tr>

            <tr class="header">
                <th><a href="javascript:void(0);" class="show" id="total-yearly-income">Total Yearly Income</a></th>
                $<td class><input id="total_yearly_income" name="total_yearly_income" type="text"  v-bind:value="getTotalYearlyIncome"></td>
            </tr>

            </tbody>
        </table>
    </div>


</template>

<script>
    import EventBus from '../app.js';
    import BootstrapVue from 'bootstrap-vue'
    export default {
        props: [''],

        data: function(){
            return {
                other_income: 0,
                monthly_income: 0,
                total_income: 0,
                yearly_income: 0,
                expense_arr: [],
                total_expenses: 0,
                rent_mortgage: 0,
                home_renters_ins: 0,
                prop_tax: 0,
                hoa_fees: 0,
                second_mortgage: 0,
                electric_gas: 0,
                home_repair: 0,
                water_sewer: 0,
                phone_cell: 0,
                cable_internet: 0,
                car_payment: 0,
                second_car_payment: 0,
                car_insurance: 0,
                gas: 0,
                parking_tolls: 0,
                groceries_household: 0,
                school_lunch: 0,
                eating_out: 0,
                health_ins_copay: 0,
                prescription: 0,
                life_ins: 0,
                clothing: 0,
                barber_shop: 0,
                dry_cleaning: 0,
                child_care: 0,
                child_support: 0,
                school_supplies: 0,
                credit_cards: 0,
                store_cards: 0,
                medical_debt: 0,
                student_loans: 0,
                tax_payments: 0,
                atm_fees: 0,
                miscellaneous_debt_payments: 0,
                monthly_subscriptions: 0,
                hobbies_sports: 0,
                news_magazines: 0,
                travel_recreation: 0,
                church_charity: 0,
                pet_care: 0,
                holiday_birthday: 0,
                other_expenses: 0,
            }
        },
        methods: {

        },
        computed: {
            getTotalMonthlyIncome: function(){
                let vm = this;
                 let running_total = vm.getTotalExpenses;
                this.total_income =  parseInt(this.other_income) + parseInt(this.monthly_income) -  parseInt(running_total);
                console.log('Monthly Income: '+ (this.monthly_income) + ' Total Income: '+ (this.other_income)+ ' = '  + this.total_income);
                return this.total_income;
            },


            getTotalYearlyIncome: function(){
                this.yearly_income =  (parseInt(this.other_income) + parseInt(this.monthly_income))  * parseInt(12);
                return this.yearly_income;
            },

            getTotalExpenses: function(){

                this.total_expenses =
                    + this.rent_mortgage +
                    + this.home_renters_ins +
                    + this.prop_tax +
                    + this.hoa_fees +
                    + this.second_mortgage +
                    + this.electric_gas +
                    + this.home_repair +
                    + this.water_sewer +
                    + this.phone_cell +
                    + this.cable_internet +
                    + this.car_payment +
                    + this.second_car_payment +
                    + this.car_insurance +
                    + this.gas +
                    + this.parking_tolls +
                    + this.groceries_household +
                    + this.school_lunch +
                    + this.eating_out +
                    + this.prescription +
                    + this.life_ins +
                    + this.clothing +
                    + this.barber_shop +
                    + this.dry_cleaning +
                    + this.child_care +
                    + this.child_support +
                    + this.school_supplies +
                    + this.credit_cards +
                    + this.store_cards +
                    + this.medical_debt +
                    + this.student_loans +
                    + this.tax_payments +
                    + this.atm_fees +
                    + this.miscellaneous_debt_payments +
                    + this.monthly_subscriptions +
                    + this.hobbies_sports +
                    + this.news_magazines +
                    + this.travel_recreation +
                    + this.church_charity +
                    + this.pet_care +
                    + this.holiday_birthday +
                    + this.other_expenses;


                //this.total_expenses =  parseInt(this.rent_mortgage) + parseInt(this.home_renters_ins) + parseInt(this.prop_tax) + parseInt(this.hoa_fees);

                //console.log('Monthly Income: '+ (this.monthly_income) + ' Total Income: '+ (this.other_income)+ ' = '  + this.total_income);
                return this.total_expenses;
            },



        },



    }
</script>
