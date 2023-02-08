<template>
<main>
    <div class="carta">
          <AlbumList/>
    </div>
</main>
</template>

<script>
import AlbumList from './albums/AlbumList.vue'

export default {
    name: 'MainComp',
    components:{
        
        AlbumList
    },

}
</script>

<style scoped lang="scss">

main{
   background-color: #3b4a58;
}

.carta{
    width: 90%;
    margin: auto;
}

</style>
