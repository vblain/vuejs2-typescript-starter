<template>
    <div>
        <p>this is app2</p>
        <p v-if="showmsg" v-bind:title="title">{{message}} {{greeting}}</p>
    </div>
</template>

<script> 
import Vue from 'vue';
export default Vue.component('app2', {
    props: ['greeting'],
    data:  () => {
        return {
            showmsg:  true,
            title:  "the title",
            message:  "Hello Vue world! "
        }
    }
});
</script>
