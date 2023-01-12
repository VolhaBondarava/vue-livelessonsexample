<template>
    <h1 v-flash="1000">Employee of the month</h1>
    <div v-if="this.personData">
        <h3 >{{ this.personData.first }} {{ this.personData.last }}</h3>
    </div>
</template>
<script>

import randomPersonMixin from '../mixins/RandomPersonMixin';
    export default {
        name: 'EmployeeOfTheMonthPage',
        mixins: [randomPersonMixin]
        
    }
</script>