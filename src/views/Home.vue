<template>
  <div class="home">
    <div class="section">
      <img src="../assets/img/bg1.png" alt="">
      <article>
        <h1>AR ЕРТӨНЦӨД ТАВТАЙ МОРИЛ</h1>
        <p>Augmented Reality буюу AR гэдэг нь програм хангамжийн тусламжтай бүтээгдсэн аливаа графикийг бодит байдалтай хослуулсан хагас бодит орчин юм. AR нь Virtual Reality-гийн хөгжлийн дараагийн үе шат юм</p>
        <button>Цааш үзэх</button>
      </article>
    </div>
    <div class="floating"><img src="../assets/img/vr.png" alt=""></div>
    <div class="home-goal">
      <article>
        <h1>Бидний зорилго</h1>
        <p>Энэхүү семинарын ажлын хүрээнд VR, түүнд ашиглагдаж буй
        техник технологи, програм хангамжийг бие даан судалж, практик
        хэрэглээнд ашиглана</p>
      </article>
      <article>
        <h1>Туршилтын нэг хэсгээс</h1>

        <iframe src="https://www.youtube.com/embed/2Q2_wTNKUms" width="100%" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <!-- <p>Хэрвээ чи мөрөөдөж чадаж байвал үүнийг хийж чадна гэсэн үг. Миний энэ бүх зүйл нэгэн мөрөөдөл болон бяцхан хулганаас эхэлсэн.</p>
        <p>-- Walter Elias "Walt" Disney</p> -->
      </article>
      <img src="../assets/img/virtual-reality2.svg" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {

  }
}
</script>

<style scoped>
  .home{
    font-family: 'Roboto Condensed', sans-serif;
    width: 100%;
  }
  .section{
    background-color: #9B59B6;
    min-height: 80vh;
    display: grid;
    grid-template-areas: "img article";
    align-items: center;
  }
  .section img {
    grid-area: img;
    height: 400px;
    margin-left: 100px;
  }
  .section article{
    grid-area: article;
    padding: 30px;
    margin-left: auto;
    margin-right: 100px;
    margin-top: -200px;
  }
  .section article h1{
    text-align: center;
    font-size: 2em;
    color: #ffffff;
    font-weight: 600;
  }
  article {
    margin: 0;
  }
  .section article p{
    text-align: right;
    width: 500px;
    color: #ffffff;
    font-size: 1.2em;
  }
  .section article button{
    background-color: #E91E63;
    border-radius: 25px;
    border: none;
    color: #ffffff;
    padding: 10px 20px;
    float: right;
  }
  button:hover{
    cursor: pointer;
    animation: animate 1s infinite;
    transition: ease-in-out 0.5s;
  }
  @keyframes animate {
    0%{
      transform: translateY(0px);
    }
    10%{
      transform: translateY(-3px);
    }
    20%{
      transform: translateY(0px);
    }
    30%{
      transform: translateY(3px);
    }
    100%{
      transform: translateY(0px);
    }
  }

  .home-goal{
    display: grid;
    align-items: center;
  }
  .home-goal article {
    width: 600px;
    margin-left: auto;
    margin-right: auto;
  }
  .home-goal article h1{
    text-align: center;
    font-size: 2em;
    color: #000;
    font-weight: 600;
  }
  .home-goal article p{
    text-align: justify;
    width: 500px;
    color: #000;
    font-size: 1.2em;
  }

  .floating img{
    width: 400px;
  }
  .floating {  
    width: 400px;
    animation-name: floating;
    animation-duration: 3s;
    animation-iteration-count: infinite;
    animation-timing-function: ease-in-out;
    position: absolute;
    right: 0;
    margin-left: auto;
    margin-right: 100px;
    margin-top: -220px;
  }
  @keyframes floating {
      from { transform: translate(0,  0px); }
      65%  { transform: translate(0, 15px); }
      to   { transform: translate(0, -0px); }    
  }



  @media only screen and (max-width: 600px) {
    .floating {
      display: none;
    }
    .section{
      width: 100%;
      grid-template-areas: "article" "img";
      justify-content: center;
    }
    .section img {
      height: 200px;
      margin-left: auto;
      margin-right: auto;
    }
    .section article{
      padding: 30px;
      margin-top: 0px;
      margin-right: auto;
      margin-left: auto;
    }
    .section article h1{
      text-align: center;
      font-size: 1.5em;
    }
    .section article p{
      text-align: center;
      width: 300px;
      color: #ffffff;
      font-size: 1em;
    }
    .section article button{
      float: left;
      margin-left: 100px;
    }
    .home-goal article {
      width: 300px;
      margin-right: auto;
      margin-left: auto;
    }
    .home-goal img {
      grid-row: 1/3;
      grid-column: 2;
      height: 300px;
      margin-top: 200px;
      margin-bottom: 50px;
      display: none;
    }
    .home-goal article h1{
      font-size: 1.4em;
    }
    .home-goal article p{
      width: 300px;
      font-size: 1em;
    }
    iframe{
      height: 200px;
      margin-bottom: 20px;
    }
  }

  /* Small devices (portrait tablets and large phones, 600px and up) */
  @media only screen and (min-width: 600px) {
    .floating {
      display: none;
    }
    .section{
      grid-template-areas: "article" "img";
      justify-content: center;
    }
    .section img {
      height: 250px;
      margin-left: auto;
      margin-right: auto;
    }
    .section article{
      padding: 30px;
      margin-top: 0px;
      margin-right: auto;
      margin-left: auto;
    }
    .section article h1{
      text-align: center;
      font-size: 1.6em;
    }
    .section article p{
      text-align: center;
      width: 400px;
      color: #ffffff;
      font-size: 1.1em;
    }
    .section article button{
      float: left;
      margin-left: 150px;
    }
    .home-goal article {
      width: 400px;
      margin-right: auto;
      margin-left: auto;
    }
    .home-goal img {
      grid-row: 1;
      height: 200px;
      margin-top: 0px;
      margin-bottom: 0px;
      display: none;
    }
    .home-goal article h1{
      font-size: 1.4em;
    }
    .home-goal article p{
      width: 400px;
      font-size: 1em;
    }
    iframe{
      height: 250px;
      margin-bottom: 40px;
    }
  }

  /* Medium devices (landscape tablets, 768px and up) */
  @media only screen and (min-width: 768px) {
    .floating {
      /* width: 200px; */
      display: inline-block;
    }
    .floating img {
      width: 200px;
    }
    .section{
      grid-template-areas: "img article" "img article";
      justify-content: center;
    }
    .section img {
      height: 300px;
      margin-left: auto;
      margin-right: auto;
    }
    .section article{
      padding: 30px;
      margin-top: -150px;
      margin-right: auto;
      margin-left: auto;
    }
    .section article h1{
      text-align: center;
      font-size: 1.8em;
    }
    .section article p{
      text-align: right;
      width: 400px;
      color: #ffffff;
      font-size: 1.2em;
    }
    .section article button{
      float: right;
    }
    .home-goal{
      grid-template-areas: "article-1 article-2" 
                           "img1 article-2";
    }
    .home-goal article {
      width: 350px;
      margin: 0;
    }
    .home-goal img {
      grid-area: img1;
      height: 250px;
      display: inline-block;
      margin-top: -180px;
      justify-self: center;
      margin-bottom: 20px;
    }
    .home-goal article:first-child{
      justify-self: center;
      grid-area: article-1;
      margin-top: -180px;
    }
    .home-goal article:last-child{
      justify-self: center;
      grid-area: article-2;
    }
    .home-goal article h1{
      font-size: 1.4em;
    }
    .home-goal article p{
      width: 300px;
      margin-left:auto;
      margin-right:auto;
      font-size: 1em;
    }
    iframe{
      height: 250px;
      margin-bottom: 20px;
    }
  }

  /* Large devices (laptops/desktops, 992px and up) */
  @media only screen and (min-width: 992px) {
    .floating {
      display: inline-block;
    }
    .floating img {
      width: 400px;
    }
    .section{
      grid-template-areas: "img article";
      align-items: center;
    }
    .section img {
      grid-area: img;
      height: 400px;
      margin-right: 70px;
    }
    .section article{
      grid-area: article;
      padding: 30px;
      margin-left: auto;
      margin-right: 0px;
      margin-top: -200px;
    }
    .section article h1{
      font-size: 2em;
    }
    .section article p{
      text-align: right;
      width: 500px;
      color: #ffffff;
      font-size: 1.2em;
    }
    .section article button{
      float: right;
    }
    .home-goal{
      align-items: center;
      grid-template-areas: "article-1 img1" 
                           "article-2 img1";
    }
    .home-goal article {
      width: 600px;
      margin-left: auto;
      margin-right: auto;
    }
    .home-goal img {
      grid-area: img1;
      height: 400px;
      margin-top: 200px;
      margin-bottom: 50px;
    }
    .home-goal article:first-child{
      justify-self: center;
      margin-top: 0;
      grid-area: article-1;
    }
    .home-goal article:last-child{
      justify-self: center;
      grid-area: article-2;
    }
    .home-goal article h1{
      font-size: 2em;
    }
    .home-goal article p{
      width: 500px;
      margin-left:auto;
      margin-right:auto;
      font-size: 1.2em;
    }
    iframe{
      height: 350px;
      margin-bottom: 20px;
    }
  } 

  /* Extra large devices (large laptops and desktops, 1200px and up) */
  @media only screen and (min-width: 1200px) {
    .floating {
      display: inline-block;
    }
  }
</style>
