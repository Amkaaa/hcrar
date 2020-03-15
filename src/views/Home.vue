<template>
  <div class="home">
    <section>
      <img src="../assets/img/bg1.png" alt="">
      <article>
        <h1>AR ЕРТӨНЦӨД ТАВТАЙ МОРИЛ</h1>
        <p>Augmented Reality буюу AR гэдэг нь програм хангамжийн тусламжтай бүтээгдсэн аливаа графикийг бодит байдалтай хослуулсан хагас бодит орчин юм. AR нь Virtual Reality-гийн хөгжлийн дараагийн үе шат юм</p>
        <button>Цааш үзэх</button>
      </article>
    </section>
    <div class="floating"><img src="../assets/img/vr.png" alt=""></div>
    <div class="team-goal">
      <article>
        <h1>Бидний зорилго</h1>
        <p>Энэхүү семинарын ажлын хүрээнд VR, түүнд ашиглагдаж буй
        техник технологи, програм хангамжийг бие даан судалж, практик
        хэрэглээнд ашиглана</p>
      </article>
      <article>
        <h1>Эшлэл</h1>
        <p>Хэрвээ чи мөрөөдөж чадаж байвал үүнийг хийж чадна гэсэн үг. Миний энэ бүх зүйл нэгэн мөрөөдөл болон бяцхан хулганаас эхэлсэн.</p>
        <p>-- Walter Elias "Walt" Disney</p>
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
  section{
    background-color: #9B59B6;
    min-height: 80vh;
    display: flex;
    align-items: center;
  }
  section img {
    height: 400px;
    margin-left: 100px;
  }
  section article{
    padding: 30px;
    margin-left: auto;
    margin-right: 100px;
    margin-top: -200px;
  }
  section article h1{
    text-align: center;
    font-size: 2em;
    color: #ffffff;
    font-family: 'Roboto Condensed', sans-serif;
    font-weight: 600;

  }
  section article p{
    text-align: right;
    width: 500px;
    color: #ffffff;
    font-family: 'Roboto Condensed', sans-serif;
    font-size: 1.2em;
  }
  section article button{
    background-color: #E91E63;
    border-radius: 25px;
    border: none;
    color: #ffffff;
    padding: 10px 20px;
    float: right;
  }
  button:hover{
    cursor: pointer;
    animation: google 1s infinite;
    transition: ease-in-out 0.5s;
  }
  @keyframes google {
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

  .team-goal{
    display: grid;
    align-items: center;
  }
  .team-goal article {
    width: 600px;
    margin-left: 50px;
  }
  .team-goal img {
    grid-row: 1/3;
    grid-column: 2;
    height: 400px;
    margin-top: 200px;
    margin-bottom: 50px;
  }
  .team-goal article:first-child{
    grid-row:1;
    grid-column: 1;
  }
  .team-goal article:last-child{
    grid-row: 1/2;
    grid-column: 1;
  }
  .team-goal article h1{
    text-align: center;
    font-size: 2em;
    color: #000;
    font-family: 'Roboto Condensed', sans-serif;
    font-weight: 600;

  }
  .team-goal article p{
    text-align: justify;
    width: 500px;
    color: #000;
    font-family: 'Roboto Condensed', sans-serif;
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
</style>
