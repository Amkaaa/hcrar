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
              <!-- Сүхбаатар дүүрэг, Их Сургуулийн гудамж, 3-р байр -->
              </h3>
            <h3 class="website"><i class="fa fa-globe" aria-hidden="true"></i><a href="/">www.mysite.mn</a></h3>
            <h3 class="email"><i class="fa fa-envelope" aria-hidden="true"></i>hrarc@gmail.com</h3>
            <h3 class="trello"><i class="fa fa-trello" aria-hidden="true"></i>Not Available Now</h3>
            <h3 class="phone"><i class="fa fa-phone-square" aria-hidden="true"></i>Not Available Now</h3>
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
    justify-self: center;
    width: 450px;
    text-align: justify;
    z-index: 999;
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
  a {
    /* color: white;
    text-decoration: none; */
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

</style>
