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
        <div class="subsribe-button">
          <button>SIGN UP NOW</button>
        </div>

        <div class="social-networks">
          <div class="follow-us">
            <p>FOLLOW US</p>
          </div>

          <div class="social-icons">

            <div class="social-button">
              <img src="../assets/footer-facebook.png" alt="">
            </div>
            
            <div class="social-button">
              <img src="../assets/footer-twitter.png" alt="">
            </div>
            
            <div class="social-button">
              <img src="../assets/footer-youtube.png" alt="">
            </div>

            <div class="social-button">
              <img src="../assets/footer-pinterest.png" alt="">
            </div>

            <div class="social-button">
              <img src="../assets/footer-periscope.png" alt="">
            </div>
        
          </div>
        </div>
      </div>
    </div>


    
  </footer>
</template>

<script>
export default {
  name: 'FooterApp',
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
    background-color: rgb(2, 130, 249);
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



  #bottom-footer{
    padding: 25px 0px;
    background-color: #303030;
    .container{
      display: flex;
      justify-content: space-between;
      align-items: center;
      .subsribe-button{
        button{
          background-color: transparent;
          border: 2px solid #0282f9;
          font-size: 14px;
          padding: 10px;
          color: white;
          &:hover{
            background-color: rgb(104, 104, 104);
            cursor: pointer;
          }
        }
      }
      .social-networks{
        display: flex;
        align-items: center;
        column-gap: 10px;
        .follow-us{
          p{
            color: #1277eb;
          }
        }
        .social-icons{
          display: flex;
          column-gap: 5px;
          .social-button{
            img{
              width: 85%;
              &:hover{
                cursor: pointer;
                width: 90%;
              }
            }
          }
        }
      }
    }
  }

</style>
