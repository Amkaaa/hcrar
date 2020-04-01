<template>
  <div class="contact">
    <div class="contact-sidebar">
      <div class="floating"> 
        <img src="../assets/img/phone2.svg" alt="">
      </div>
      <img src="../assets/img/phone1.svg" alt="">  
    </div>
    <div class="contact-us">
        <h1>Бидэнтэй холбоо барих</h1>
        <div class="contact-us-info">
            <h3 class="contact-address"><i class="fa fa-location-arrow" aria-hidden="true"></i>
              МУИС ХШУИС, 
              14201 Улаанбаатар хот-46а ш/х-600
              </h3>
            <h3 class="contact-address" style="margin-left: 50px;">Сүхбаатар дүүрэг, Их Сургуулийн гудамж, 3-р байр</h3>
            <h3 class="website"><i class="fa fa-globe" aria-hidden="true"></i><a href="/">https://humancomputer.me/</a></h3>
            <h3 class="email"><i class="fa fa-envelope" aria-hidden="true"></i>99061017a@gmail.com</h3>
            <h3 class="trello"><i class="fa fa-trello" aria-hidden="true"></i>Trello</h3>
            <h3 class="phone"><i class="fa fa-phone-square" aria-hidden="true"></i>+(976) 95829514</h3>
        </div>
    </div>
    <svg id="svg" xmlns="http://www.w3.org/2000/svg" viewBox="-300 0 950 270" >
    <path d="M-314,267 C105,364 400,100 812,279" fill="none" stroke="white" stroke-width="120" stroke-linecap="round"/>
  </svg>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Contact',
  components: {

  }
}
</script>

<style scoped>
  svg {
    position: absolute;
    bottom: 40px;
    width: 100%;
    height: auto;
  }
  .contact{
      min-height: calc(100vh - 115px);
      font-family: 'Roboto Condensed', sans-serif;
      background: #E91E63;
      display: grid;
      grid-template-areas: "sidebar us us" 
                            "sidebar us us";
  }
  .contact-sidebar{
    grid-area: sidebar;
    justify-self: center;
    align-self: center;
  }
  .contact-us{
    grid-area: us;
    justify-self: flex-start;
    margin-left: 10px;
    width: 450px;
    text-align: justify;
    z-index: 0;
  }
  .contact-sidebar img{
    width: 400px;
    height: 400px;
  }
  h1 {
    color: #ffffff;
    font-weight: 500;
    font-size: 2.5em;
  }
  .fa {
    font-size: 1.8em;
    color: #ffffff;
    margin-right: 20px;
  }
  h3 {
    color: #ffffff;
    font-weight: 100;
  }
  a:hover{
    opacity: 0.8;
  }

  .floating {  
    width: 400px;
    animation-name: floating;
    animation-duration: 2s;
    animation-iteration-count: infinite;
    animation-timing-function: ease-in-out;
    position: absolute;
  }

  @keyframes floating {
      from { transform: translate(0,  0px); }
      65%  { transform: translate(0, 15px); }
      to   { transform: translate(0, -0px); }    
  }

  /* Extra small devices (phones, 600px and down) */
  @media only screen and (max-width: 600px) {
    .contact {
      grid-template-areas: "us" "sidebar";
      min-height: calc(100vh - 95px);
    }
    .contact-sidebar{
      margin-top: -350px;
      margin-left: 300px;
    }
    .contact-sidebar img{
      width: 150px;
      height: 150px;
    }
    .floating {
      width: 150px;
    }
    svg {
      bottom: 40px;
    }
  }

  /* Small devices (portrait tablets and large phones, 600px and up) */
  @media only screen and (min-width: 600px) {
    .contact {
      grid-template-areas: "us" "sidebar";
      min-height: calc(100vh - 95px);
    }
    .contact-sidebar{
      margin-top: -350px;
      margin-left: 300px;
    }
    .contact-sidebar img{
      width: 150px;
      height: 150px;
    }
    .floating {
      width: 150px;
    }
    svg {
      bottom: 40px;
    }
  }

  /* Medium devices (landscape tablets, 768px and up) */
  @media only screen and (min-width: 768px) {
    .contact {
      grid-template-areas: "sidebar us us" 
                            "sidebar us us";
      min-height: calc(100vh - 115px);
    }
    .contact-sidebar{
      margin-top: -100px;
      margin-right: auto;
      margin-left: auto;
    }
    .contact-sidebar img{
      width: 300px;
      height: 300px;
    }
    .floating {
      width: 300px;
    }
    svg {
      bottom: 40px;
    }
  } 

  /* Large devices (laptops/desktops, 992px and up) */
  @media only screen and (min-width: 992px) {
    .contact {
      grid-template-areas: "sidebar us us" 
                            "sidebar us us";
      min-height: calc(100vh - 115px);
    }
    .contact-sidebar{
      margin-top: -100px;
      margin-right: auto;
      margin-left: auto;
    }
    .contact-sidebar img{
      width: 350px;
      height: 350px;
    }
    .floating {
      width: 300px;
    }
    svg {
      bottom: 40px;
    }
  } 

  /* Extra large devices (large laptops and desktops, 1200px and up) */
  @media only screen and (min-width: 1200px) {
    .contact {
      grid-template-areas: "sidebar us us" 
                            "sidebar us us";
      min-height: calc(100vh - 115px);
    }
    .contact-sidebar{
      margin-top: -100px;
      margin-right: auto;
      margin-left: auto;
    }
    .contact-sidebar img{
      width: 400px;
      height: 400px;
    }
    .floating {
      width: 300px;
    }
    svg {
      bottom: 40px;
    }
  }
</style>
