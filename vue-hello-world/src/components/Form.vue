<template>
    <h1>testasndo o form</h1>
    <InputText/>
    <InputText/>
    <Submit/>
</template>
<script>

import InputText from './form/inputText.vue';
import Submit from './form/Submit.vue'

    export default {
        name:'Form',
        components: {
            InputText,
            Submit,
        }
    }
</script>