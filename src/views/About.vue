<template>
  <div class="about">
      <div class="about-sidebar"><img src="../assets/img/bg2.png" alt=""></div>
      <div class="about-us">
        <h1>Бидний тухайд</h1>
        <p>Манай баг нь <strong>Хүн ба Компьютерийн харилцаа (ICSI440)</strong> хичээлийн Баасан 11:00 цагийн семнарын баг. Бид энэхүү хичээлээр Хагас бодит байдал буюу Augmented Reality гэсэн сэдвийг судлаж байна.</p>
      </div>
      <div class="about-team">
        <div class="team-member">
          <img src="../assets/profile/amraa.jpg" alt="">
          <h3>Г. Амартайван</h3>
          <h4>Би МУИС-д Програм Хангамжийн чиглэлээр суралцдаг 4-р курсийн оюутан. Дата аналитик, AR, өгөгдлийн бүтэц, машин сургалт, VueJS-д сонирхолтой.</h4>
          <h4><i class="fa fa-envelope-o" aria-hidden="true"></i> 99061017a@gmail.com</h4>
          <div class="team-member-social">
            <a class="nonactive"><i class="fa fa-facebook-square" aria-hidden="true"></i></a>
            <a href="https://amkaaa.github.io/amka.github.io/" target="_blank"><i class="fa fa-github-alt" aria-hidden="true"></i></a>
            <a href="https://www.linkedin.com/in/amartaivan-ganbat-771469175/"  target="_blank"><i class="fa fa-linkedin-square" aria-hidden="true"></i></a>
          </div>
        </div>
        <div class="team-member">
          <img src="../assets/profile/nyamaa.jpeg" alt="">
          <h3>Э. Нямжанцан</h3>
          <h4>Би энэ жил МУИС-н төгсөх курсийн оюутан. Би багаасаа дизайн график талдаа сонирхолтой байсан учраас бие дааж AR технологийг судалдаг. AR бол зүгээр л гайхамшиг.</h4>
          <h4><i class="fa fa-envelope-o" aria-hidden="true"></i> sstrby@gmail.com</h4>
          <div class="team-member-social">
            <a class="nonactive"><i class="fa fa-facebook-square" aria-hidden="true"></i></a>
            <a class="nonactive"><i class="fa fa-github-alt" aria-hidden="true"></i></a>
            <a class="nonactive"><i class="fa fa-linkedin-square" aria-hidden="true"></i></a>
          </div>
        </div>
        <div class="team-member">
          <img src="../assets/profile/lhamaa.jpeg" alt="">
          <h3>Р. Лхамсүрэн</h3>
          <h4>Өнөө цагийн технологийн дэвшил гэж юуг ойлгох вэ? гэвэл би AR-г хэлнэ. AR-н ачаар бид бодит ертөнцөд боломжгүй зүйлсийг боломжтой болгож чадаж байна.</h4>
          <h4><i class="fa fa-envelope-o" aria-hidden="true"></i>chebrush21@gmail.com</h4>
          <div class="team-member-social">
            <a class="nonactive"><i class="fa fa-facebook-square" aria-hidden="true"></i></a>
            <a class="nonactive"><i class="fa fa-github-alt" aria-hidden="true"></i></a>
            <a class="nonactive"><i class="fa fa-linkedin-square" aria-hidden="true"></i></a>
          </div>
        </div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'About',
  components: {
    
  }
}
</script>

<style scoped>
    .about {
        min-height: calc(100vh - 115px);
        background: #F1C40F;
        font-family: 'Roboto Condensed', sans-serif;
        display: grid;
        grid-template-areas: "sidebar us us"
                             "sidebar team team "
                             "sidebar team team";
    }
    .about img {
      width: 400px;
      height: 400px;
    }
    .about-sidebar{
      margin: 40px;
      grid-area: sidebar;
      justify-self: center;
      align-self: center;
    }
    .about-us{
      grid-area: us;
    }
    .about-team{
      padding: 0px 40px;
      grid-area: team;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      text-align: center;
    }
    .about-team .team-member{
      background: #2C3E50;
      box-shadow: 5px 5px 5px rgb(0,0,0,0.5);
      height: 415px;
      width: 250px;
    }
    .about-team img{
      padding: 15px 10px 10px;
      width: 200px;
      height: 200px;
      object-fit: cover;
    }
    h1{
      color: #2C3E50;
      font-weight: 600;
      font-size: 2.8em;
      margin: 10px 0;
      text-align: center;
    }
    h3{
      margin: 0;
      color: #f5f5f5;
      font-weight: 500;
      margin-bottom: 10px;
    }
    h4{
      margin: 0 20px 0 20px;
      text-align: justify;
      font-size: 0.8em;
      font-weight: 100;
      margin-bottom: 10px;
      color: white;
    }
    h4 .fa{
      margin-right: 20px;
    }
    p {
      margin: 0 20px 0 20px;
      text-align: justify;
      font-size: 0.9em;
    }
    .team-member-social .fa {
      color: #E91E63;
      font-size: 2em;
      margin-right: 10px;
      margin-left: 10px;
    }
    .team-member-social .nonactive {
      color: #E91E63;
      opacity: 0.5;
      user-select: none;
    }
</style>