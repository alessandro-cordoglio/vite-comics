<script>


export default {
  data(){
    return{
      items:[
              {
                image: 'buy-comics-digital-comics.png',
                info:'DIGITAL COMICS'
              } ,
              {
                image: 'buy-comics-merchandise.png',
                info:'DC MERCHANDISE'
              } ,
              {
                image: 'buy-comics-subscriptions.png',
                info:'SUBSCRIPTION'
              } ,
              {
                image: 'buy-comics-shop-locator.png',
                info:'COMIC SHOP LOCATOR'
              } ,
              {
                image: 'buy-dc-power-visa.svg',
                info:'DC POWER VISA'
              } ,
            ]
    }

  },
  components: {
   
  }
}
</script>

<template>
  <section class="item_section">
    <div class="container_">
      <div class="items">
        <div class="item"  v-for="item in items">
          <div class="item_image">
            <img :src="'/src/assets/'+ item.image" alt="">
          </div>
          <div class="item_info">{{item.info}}</div>
        </div>
      </div>
    </div>
  </section>
  <section class="small_info--section">
    
  </section>
</template>

<style lang="scss" scoped>
  .items, .item{
    display: flex;
    align-items: center;
    justify-content: space-between;
    .item{
      padding: 40px 20px;
      color: white;

      .item_info{
        font-size: 14px;
        margin-left: 10px;
      }
      img{
        width: 40px;
      }
    }
  }
</style>