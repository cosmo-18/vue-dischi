<template>
<div class="list">

    <AlbumCard v-for="(elem, index) in albums" :key="index" :nomeProps="elem"/>


</div>
</template>

<script>

import AlbumCard from './AlbumCard.vue'
import axios from 'axios';

export default {
    name: 'AlbumList',
    components:{

        AlbumCard
    },
    data(){
        return{
            albums:[

            ]
        }
    },
    // *  carica le informazioni al caricamento della pagina * //
    mounted(){
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response)=>{
            this.albums =response.data.response

            })
            
    },


}
</script>

<style scoped lang="scss">

.list{
    display: flex;
    flex-wrap: wrap;
    align-content: center;
    justify-content: space-around;
    padding: 20px;
}

</style>