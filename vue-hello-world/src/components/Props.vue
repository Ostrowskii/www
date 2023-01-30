<template>
    <div>
        <button @click="AddFavoritos">{{ buttonName }}</button>
    </div>
    <p v-show="like">gosto dessa cor</p>
</template>
<script>
    export default { 
        name: 'Props',
        props: {
            buttonName: String,
        },
        data(){
            return{
                like: false,
                listaCorFavorita: [],
            }
        },
        methods: {
            AddFavoritos(){
                this.like = !this.like;
                // console.log(this.like);
                // this.listaCorFavorita.push(this.buttonName)
                // if (this.listaCorFavorita.prototype.indexOf(this.buttonName)) {
                //     console.log("tem sim");
                //     console.log(this.listaCorFavorita);
                // }
            }
        }
    }
</script>