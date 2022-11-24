<!-- SCRIPT -->
<script>
export default {
    data(){
       return{
            links:[
                "CHARACTERS",
                "COMICS",
                "MOVIES",
                "TV",
                "GAMES",
                "COLLECTIBLES",
                "VIDEOS",
                "FANS",
                "NEWS",
                "SHOP"
            ]     
       }
    },
    components: {
   
  }
}
</script>

<!-- TEMPLATE -->
<template>
    <div class="container_ header_container">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="">
        </div>
        <nav class="nav_layout">
            <ul>
                <li v-for="link in links"><a href="#">{{link}}</a></li>
            </ul>
        </nav>
    </div>
</template>

<!-- STYLE -->
<style lang="scss" scoped>
    .header_container{
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .nav_layout{
        height: 100%;
    }
</style>