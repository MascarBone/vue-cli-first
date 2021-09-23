<template>
  <div>
      <div class="container">
          <div class="bg-img">
              <h1>This is a preview for a content</h1>
              <h2>{{text}}</h2>
              <div class="wrapper">
                  <div class="side side-left">
                        <p>Content on the left</p>
                  </div>
                  <div class="side side-left">
                        <p>Content still on the left</p>
                  </div>
                  <div class="side side-right">
                        <p>This is the right side of the page</p>
                  </div>
              </div>

              <div class="flexxer">
                  <div class="row">
                      <div class="col">
                          <span>Parte di una colonna</span> 
                      </div>
                      <div class="col">
                          <span>Parte di una colonna</span> 
                      </div>
                      <div class="col">
                          <span>Parte di una colonna</span> 
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Hero',
    props: {
        text: String,
    }

}
</script>

<style scoped>
    * {
        color: white;
    }
    h1 {
        padding: 20px 0;
    }
    .container{
        /* color: white; */
        width: 1200px;
        margin: 0 auto;
    }    
    .bg-img {
        background-image: url('https://sm.ign.com/ign_it/screenshot/default/kena-bridge-of-spirits-hero_4s8j.jpg');
        /* background-size: cover; */
        background-position: center;
        /* width: 1280px;
        height: 720px; */

    }
    .wrapper::after {
    content: "";
    display: table;
    clear: both;
    }
    .side {
        font-size: 2rem;
        margin: 0 10px;
    }
    .side-left {
        float: left;
    }
    .side-right {
        float: right;
    }
    .flexxer {
        display: flex;
    }
    .row {
        display: flex;
        width: 100%;
        justify-content: space-evenly;
    }
    .col {
        width: 18%;
        padding: 50px 0;
        font-size: 3rem ;
    }
</style>