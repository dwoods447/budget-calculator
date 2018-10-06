<template>
    <div class="row">
        <input type="text" :id="idText+dynamicID()">
    </div>
</template>

<script>
    export default {
        data: function () {
           return {
               classValue: 'red',
               idText: 'input-id-',
               timesClicked: 1,
           }
        },
        methods: {

        },
        mounted() {
            console.log('Input Component mounted.')
        }
    }
</script>
