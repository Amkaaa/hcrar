<template>
  <div class="assignment">
      <div class="assign-description">
        <h2>
          Ажлын талбар
        </h2>
        <p>
          Манай багийн хөгжүүлж байгаа ажлын хэсэг
        </p>
      </div>
      <div class="assign-presentation">
        <h3>Судалгаа</h3>
        <ul>
          <li>
            <h4>Товч танилцуулга</h4>
            
            <img src="../assets/img/slideshare-brands.svg" alt="">
            <h5>Судалгааны ажил  №1</h5>
              
            <p>
              Энэхүү ажлаар бид Augmented Reality-ийн тухай танилцаж, түүний тухай судалгаа хийж үзсэн.
            </p>
            
            <div class="btn">
              <a href="" download>Татаx</a>
              <a href="" target="_blank">Үзэх</a>
            </div>
          </li>
        </ul>
      </div>
      <div class="assign-assignment">
        <h3>Даалгавар</h3>
        <ul>
          <li>
            <h4>Товч танилцуулга</h4>
            
            <img src="../assets/img/edit-solid.svg" alt="">
            <h5>Даалгавар №1</h5>
              
            <p>
              Гэртээ байгаа 3-н интерфэйсийг судлаж, сул болон давуу тал, мөн сайжруулах зүйлсийг бичих. 
            </p>
            <div class="btn">
              <p><strong><i class="fa fa-download" aria-hidden="true"></i> Татах</strong></p>
              <a href="../../files/assign01_amraa.pdf" target="_blank" >Амартайван</a>
              <a href="../../files/assign01_lhamaa.pdf" target="_blank" >Лхамсүрэн</a>
              <a href="../../files/assign01_nyamaa.pdf" target="_blank" >Нямжанцан</a>
            </div>
          </li>
        </ul>
      </div>
      <div class="assign-reference">
        <h3>Холбогдох материал</h3>
        <ul>
          <li>
            <h5>Судалгааны ажилтай холбоотой нэмэлт материалууд</h5>
            <img src="../assets/img/globe-solid.svg" alt="">
            <h5><a href="https://boundlessworkspace.weebly.com/" target="_blank">Дэлгэрэнгүй</a></h5>
          </li>
        </ul>
      </div>
      <div class="assign-sidebar">
        <img src="../assets/img/virtual-reality2.svg" alt="">
      </div>
  </div>
</template>

<script>
export default {
  name: 'Assignment',
  components: {

  }
}
</script>

<style scoped>
    .assignment {
        min-height: calc(100vh - 115px);
        background: #27AE60;
        display: grid;
        grid-template-areas: "description description sidebar"
                             "presentataion assignment sidebar"
                             "reference . sidebar";
        font-family: 'Roboto Condensed', sans-serif;
    }
    ul {
      width: 20em;
      padding: 0;
      margin: auto;
    }
    ul li {
      list-style: none;
      /* border: 1px solid black; */
      padding: 10px 15px;
    }
    ul li img{
      height: 3em;
    }
    ul li .btn {
      margin-left: 80px;
      margin-right: auto;
      margin-top: 70px;
    }
    ul li .btn a {
      margin-right: 10px;
      border: 1px solid black;
      padding: 5px 10px;
      text-decoration: none;
      color: #ffffff;
      background: #E91E63;
      border-radius: 25px;
      display: inline-block;
    }
    ul li .btn a:hover {
      transform: translateY(-5px);
      transition: ease 1s;
    }
    .assign-description{
      grid-area: description;
      margin-left: auto;
      margin-bottom: 20px;
    }
    .assign-presentation{
      grid-area: presentataion;
    }
    .assign-reference{
      margin-bottom: 50px;
      grid-area: reference;
    }
    .assign-assignment{
      grid-area: assignment;
    }
    .assign-sidebar{
      grid-area: sidebar;
      justify-self: center;
      align-self: center;
    }
    .assign-sidebar img{
      width: 400px;
      height: 400px;
    }
    h2{
      text-align: center;
      margin-top: 1.5em;
      font-size: 3.5em;
      margin: 0;
      margin-top: 20px;
    }
    ul li p{
      vertical-align: middle;;
      text-align: justify;
      float: right;
      color: #111;
    }
    p{
      margin: 0;
      font-size: 1em;
      color: #fff;
      text-align: center;
    }
    h3{
      margin: 0;
      font-size: 2em;
      margin-top: 50px;
      text-align: center;
    }
    h4{
      margin: 0;
      padding: 0;
      font-size: 1.2em;
      margin-bottom: 10px;
    }
    h5{
      float: right;
      font-size: 1em;
      padding-top:10px;
      margin: 0;
    }
    .btn p {
      margin-bottom: 10px;
      margin-left: 25px;
    }
    .assign-assignment .btn{
      margin: 70px 0 0 0 ;
      display:flex;
      flex-direction: column;
    }
    .assign-assignment .btn a{
      width: 6em;
      text-align: center;
      margin-bottom: 10px;
    }
    .assign-reference h5{
      margin-bottom: 10px;
    }
    .assign-reference a{
      text-decoration: none;
      vertical-align: middle;
      transition: ease-in-out 0.2s;
    }
    .assign-reference a:hover{
      color: #E91E63;
    }
    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
      .assignment {
        grid-template-areas: "description" "sidebar" "presentataion" "assignment" "reference";
      }
      .assign-description{
        margin-left: auto;
        margin-right: auto;
      }
      .assign-sidebar img{
        width: 200px;
        height: 200px;
      }
      p {
        font-size: 1.2em;
      }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 600px) {
      .assignment {
        grid-template-areas: "description" "sidebar" "presentataion" "assignment" "reference";
      }
      .assign-description{
        margin-left: auto;
        margin-right: auto;
      }
      .assign-sidebar img{
        width: 300px;
        height: 300px;
      }
      p {
        font-size: 1.4em;
      }
      .fa-download{
        margin-top: 50px;
      }
      h5{
        float: right;
        font-size: 1.2em;
        padding-top:10px;
        margin: 0;
      }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) {
      .assignment {
        grid-template-areas: "description description" 
                             "sidebar sidebar" 
                             "presentataion assignment" 
                             "reference assignment";
      }
      .assign-sidebar img{
        width: 300px;
        height: 300px;
      }
      p {
        font-size: 1.4em;
      }
      .fa-download{
        margin-top: 50px;
      }
      h5{
        float: right;
        font-size: 1.2em;
        padding-top:10px;
        margin: 0;
      }
    } 

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) {
      .assignment {
        grid-template-areas: "description description sidebar"
                             "presentataion assignment sidebar"
                             "reference . .";
      }
      .assign-description{
        margin-left: auto;
        margin-right: auto;
      }
      .assign-sidebar img{
        width: 300px;
        height: 300px;
      }
      p {
        font-size: 1.2em;
      }
      .fa-download{
        margin-top: 0px;
      }
      h5{
        float: right;
        font-size: 1.2em;
        padding-top:10px;
        margin: 0;
      }
    } 

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {
      .assignment {
        grid-template-areas: "description description sidebar"
                             "presentataion assignment sidebar"
                             "reference . .";
      }
      .assign-description{
        margin-left: auto;
        margin-right: auto;
      }
      .assign-sidebar img{
        width: 300px;
        height: 300px;
      }
      p {
        font-size: 1.2em;
      }
      h5{
        float: right;
        font-size: 1.2em;
        padding-top:10px;
        margin: 0;
      }
    }

</style>