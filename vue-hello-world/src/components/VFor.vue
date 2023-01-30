<template>
    <h1>V for com listagem </h1>
    <ul>
        <li v-for="(technology, index) in backend" v-bind:key="index" >{{ technology }}</li>
    </ul>
    <h1>front end</h1>
    <ul>
        <li v-for="technology in frontend" :key="technology.id">
            {{ technology.language }}
        </li>
    </ul>
</template>
<script>
    export default {
        name: 'VFor',
        data(){
            return {
                backend: ['JavaScript', 'PHP', 'Python'],
                frontend: [
                    {id: 1, language:'HTML'},
                    {id: 1, language:'CSS'},
                    {id: 1, language:'Vue'},
                ],
            }
        },
    }
</script>