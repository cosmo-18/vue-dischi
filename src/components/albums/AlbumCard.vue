<template>
  <div id="cardischi">
  <div class="car col-3" style="width: 18rem;">
  <img :src="nomeProps.poster" class="card-img-top" alt="...">
  <div class="card-body">
    <div class="font">
    <h5 class="card-title">{{nomeProps.title}}</h5>
    <h5 class="card-text">{{nomeProps.author}}</h5>
    <h5 class="card-text">{{nomeProps.genre}}</h5>
    </div>
  </div>
</div>
</div>
</template>

<script>

export default {
  name: 'AlbumCard',
  props:{
    nomeProps: Object
  }

}
</script>

<style lang="scss">

#cardischi{

    border: none;
    padding: 20px;

}

.card-body{
    width: 100%;
    border: none;
    background-color: #2E3A46;
}



.font{
    color: white;
    width: 100%;
    font-size: 10px;

    }






</style>