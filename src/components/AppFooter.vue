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
            ],
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
    <div class="container_ small_info">
      <div class="left_footer">
        <div class="info_block first_info">
          <div class="info_list">
            <div class="info_title">
              <h3>DC COMICS</h3>
            </div>
            <div>
              <ul class="list_elements">
                <li><a href="#">Characters</a></li>
                <li><a href="#">Chara</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Cacters</a></li>
                <li><a href="#">Charars</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Charaters</a></li> 
              </ul>
            </div>
          </div>
          <div class="first_info--second_block">
            <div class="info_list">
            <div class="info_title ">
              <h3>SHOP</h3>
            </div>
            <div>
              <ul class="list_elements">
                <li><a href="#">Characters</a></li>
                <li><a href="#">Chara</a></li>
                <li><a href="#">Characters</a></li>
              </ul>
            </div>
          </div>
          </div>
        </div>
        <div class="info_block second_info">
          <div class="info_list">
            <div class="info_title">
              <h3>DC</h3>
            </div>
            <div>
              <ul class="list_elements">
                <li><a href="#">Characters</a></li>
                <li><a href="#">Chara</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Cacters</a></li>
                <li><a href="#">Charars</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Charaters</a></li> 
                <li><a href="#">Cacters</a></li>
                <li><a href="#">Charars</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Charaters</a></li> 
              </ul>
            </div>
          </div>
        </div>
        <div class="info_block third_info">
          <div class="info_list">
            <div class="info_title">
              <h3>SITES</h3>
            </div>
            <div>
              <ul class="list_elements">
                <li><a href="#">Characters</a></li>
                <li><a href="#">Chara</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Cacters</a></li>
                <li><a href="#">Charars</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Charaters</a></li> 
              </ul>
            </div>
          </div>
        </div>
      </div>

      <div class="right_footer">
        <div class="right_footer_bg">
          <img src="../assets/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
  </section>
  <section class="sign_up--section">
    <div class="container_ sign_up">
      <div class="sign_up--left">
        <div class="btn">
          <button class="main_button">
              SIGN-UP NOW!
          </button>
        </div>
      </div>
      <div class="sign_up--right">
        <div class="sign_up--title">
          <span>FOLLOW US</span>
        </div>
        <div class="sign_up_social flex">
          <div><img src="../assets/footer-facebook.png" alt=""></div>
          <div><img src="../assets/footer-twitter.png" alt=""></div>
          <div><img src="../assets/footer-youtube.png" alt=""></div>
          <div><img src="../assets/footer-pinterest.png" alt=""></div>
          <div><img src="../assets/footer-periscope.png" alt=""></div>
         
        </div>
      </div>
    </div>
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

  .small_info{
    display: flex;
    justify-content: space-between;
    max-height: 450px;
    align-items: center;
  }
  .left_footer{
    display: flex;
    padding-top: 40px ;
    padding-bottom: 60px;
    .info_title{
      color: white;
    }
  }
  .first_info--second_block{
    margin-top: 20px;
  }
  .info_block{
    padding: 0px 20px;
  }
  .btn{
    padding: 30px 0px;
  }
  .sign_up{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .sign_up--right{
      display: flex;
      .sign_up--title{
        color: var(--backgroundcolor-secondary);
        font-weight: bold;
        font-size: 24px;
      }
      .sign_up_social{
        img{
          margin-left:15px ;
        }
      }
    }
  }
</style>