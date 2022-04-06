<template>
  <footer>
    

    <!-- Footer superiore con le varie opzioni -->
    <div id="top-footer">
      <div class="container">

        <div class="info-item">
          <div class="logo-info">
            <img src="../assets/buy-comics-digital-comics.png" alt=""> 
          </div>
          
          <span>DIGITAL COMICS</span>
        </div>

        <div class="info-item">
          <div class="logo-info">
            <img src="../assets/buy-comics-merchandise.png" alt=""> 
          </div>
          
          <span>DC MERCHANDISE</span>
        </div>

        <div class="info-item">
          <div class="logo-info">
            <img src="../assets/buy-comics-subscriptions.png" alt=""> 
          </div>
          
          <span>SUBSCRIPTION</span>
        </div>

        <div class="info-item">
          <div class="logo-info">
            <img src="../assets/buy-comics-shop-locator.png" alt=""> 
          </div>
          
          <span>COMIC SHOP LOCATOR</span>
        </div>

        <div class="info-item">
          <div class="logo-info">
            <img src="../assets/buy-dc-power-visa.svg" alt=""> 
          </div>
          
          <span>DC POWER VISA</span>
        </div>

      </div>
    </div>

    <!-- footer centrale con i link per le altre pagine -->
    <div id="links-footer">
      <div class="container">
        <div class="links-box">
          <div class="links-item">
            <p>DC COMICS</p>
            <ul>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
            </ul>
          </div>
          <div class="links-item">
            <p>DC</p>
            <ul>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
            </ul>
          </div>
          <div class="links-item">
            <p>SITES</p>
            <ul>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
            </ul>
          </div>

          <div class="links-item">
            <p>SHOP</p>
            <ul>
              <li><a href="#">Lorem</a></li>
              <li><a href="#">Lorem</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>


    <!-- Footer inferiore con i link per i social network -->
    <div id="bottom-footer">
      <div class="container">

      </div>
    </div>


    
  </footer>
</template>

<script>
export default {
  name: 'FooterApp',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  ul{
    li{
      list-style-type: none;
    }
  }

  #top-footer{
    background-color: #0282f9;
    .container{
      display: flex;
      font-size: 11px;
      justify-content: center;
      //column-gap: 10px;
      padding: 40px 0px;
      color: white;
      .info-item{
        width: calc(100% / 5);
        display: flex;
        align-items: center;
        .logo-info{
          width: 40%;
          display: flex;
          justify-content: center;
          img{
          max-width: 50px;
       
        }
      }
      
    }
    }

  }

  #links-footer{
    padding: 50px 0px;
    
    background-image: url('../assets/footer-bg.jpg');
    .container{
      display: flex;
      .links-box{
        display: flex;
        width: 46%;
        flex-wrap: wrap;
        .links-item{
          width: calc(100% / 3);
          p{
            font-size: 18px;
            color: white;
          }
          ul{
            line-height: 20px;
            li{
              a{
                text-decoration: none;
                color: gray;
                font-size: 14px;
                &:hover{
                  color: white;
                }
              }
            }
          }
        }
      }
    }
  }
</style>
