<script>
// import { defaultServerMainFields } from 'vite';

    export default { 
        // Add Code Here
        // challenge: use array
        data() {
            return {
                message: "Choose your favourite fruit",
                fruit1: "Durian",
                fruit2: "Apple",
                fruit3: "Banana",
                fruits: ["apple", "orange", "peach"]
            }
        }  
    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
        <h3>Using Array</h3>
        {{ message }}</br>
        <!-- v- is a vue built-in function -->
        <span v-for="fruit in fruits">
            {{ fruit }}<input type='radio' name ='fruit'>
        </span>
    </div>
</template>

<style scoped>
</style>
