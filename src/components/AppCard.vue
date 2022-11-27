<script>
export default {
    props:{
        img:String,
        did:String,
    },
  components: {
  }
}
</script>

<template>
    <div class="card">
        <div class="card_img">
            <img :src="img"  :alt="did">
            <span>{{did}}</span>
        </div>
        
       
    </div>
</template>

<style lang="scss" scoped>
    .card{
       padding: 30px 0px;
        .card_img{
            img{
            width: 100%;
            height: 210px;
            object-fit: cover;
        }
        }
    }
</style>
