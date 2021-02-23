<template>
  <div id="app" >
    <Navbar v-bind:boxSvg="boxSvg" />
       <div class="row wrapper" >
              <div class="col-md-12">
                  <div class="content">
                    <h1 class="font-weight-bold">Make your <br> website  better. <br> <span class="color-green">Instantly</span></h1>
                      <div class="card w-75">
                        <div class="card-body">
                          <p class="card-text">Over 300,000 websites use Crazy Egg to improve what's working, fix what isn't and test new ideas.</p>
                            <form class="form-inline">
                              <input class="form-control " type="search" placeholder="Enter your website URL" aria-label="Search">
                              <button class="btn btn-info card-btn " type="submit">Show me my Heatmap</button>
                            </form>
                          <p class="last-p">Start your 30-day FREE trial  •  Cancel anytime</p>
                        </div>
                        
                      </div>
                    

                </div>
                
                 <p class="not-ready">
                      <a href="">Not ready to get started? Learn more</a>
                  </p>
              </div>
          </div>
    <main class="bg-image" :style="{'background-image': `url(${mySvgBg})`}">
       
    </main>
  </div>
</template>

<script>
import Navbar from './components/navbar'

export default {
  name: 'App',
  components:{
    Navbar
  },
  data(){
    return{
      mySvgBg: require('./assets/hill.svg'),
      boxSvg: require('./assets/ballon.svg')
        
    }
  }
}
</script>

<style>
  *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  
  h1{
      margin-bottom: 20px !important;
      color: #004573;
      margin-left: 50px;
      letter-spacing: 2.5px !important;
   }
  .bg-image{
    height: 120px;
    background-repeat: no-repeat;
    background-size: cover;
  }
  .content{
     margin-top: 20px;
        margin-left: 160px;
        margin-right: 100px;
  }
  .card{
    background-color: #004573 !important;
    color: white;
    padding: 15px;
    border-color: #004573 !important;
    margin-bottom: 20px;
  }
  .card-text{
    font-size: 1.2rem;
    margin-bottom: 2.5rem;
  }
  
  p{
    font-family: proxima-nova,Nunito,-apple-system,system-ui,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Arial,sans-serif;
  }
  
  .last-p{
    color: #fff;
    margin-bottom: 1.2;
    font-size: 14px;
    margin-top: 20px;
  }
  
    
    form .card-btn{
      background: #0079d0 !important;
      border: 0 !important;
      overflow: hidden !important;
      position: relative !important;
      padding: 19px 30px 19px 30px;
      border-left: 0px !important;
      border-radius: 1px !important;

    }
  
   form input {
    border-right: 0px !important;
    border-radius: 1px !important;
    padding: 30px 10px 30px 25px !important;
    text-align: left !important;
  }
   
   .wrapper{
      width: 70% !important;
      margin: 0 auto !important;
     
   }
   
   .color-green{
     color: lawngreen !important;
   }


  .not-ready  {
      margin-top: 30px !important;
      margin-left: 300px !important;
    }
  
  a{
          color: #004573 !important;

  }
  

</style>
