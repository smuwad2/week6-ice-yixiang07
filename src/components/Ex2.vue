<script>
    export default { 
        data() {
            return {
                width: '200',
                height: '200',
                myImg: '/assets/me.png'
            }
        },
    }
</script>

<template>

    <!-- add code here -->
   <img :src="myImg" :width="width" v-bind:height="height">
   <!-- optional to put v-bind: or just : is fine -->
</template>
