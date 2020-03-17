<template>
    <div class="header">
        <a href="/">
            <div class="logo">
            <img src="../../assets/logo/ar.svg" alt="">
            <p>Augmented Reality</p>
        </div>
        </a>
        <div class="navbar">
            <div class="main" v-on:click="change" v-class="{active: isActive}"> 
                <div class="bar1"></div>
                <div class="bar2"></div>
                <div class="bar3"></div>
            </div>
            <div class="navbar-link">
                <span class="home">
                    <img src="../../assets/img/icons8-augmented-reality-64.png">
                    <router-link to="/" >НҮҮР</router-link>
                </span>
                <router-link to="/Assignment">Бие даалт</router-link>
                <router-link to="/About">Бидний тухай</router-link>
                <router-link to="/Contact">Холбоо барих</router-link>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "Header"
}
</script>

<style lang="css" scoped>
    .main{
        position: absolute;
        right: 20px;
        display: inline-block;
        cursor: pointer;
    }
    .bar1, .bar2, .bar3 {
        width: 30px;
        height: 4px;
        background-color: #333;
        margin: 5px 0;
        transition: 0.4s;
    }
    .change .bar1 {
        -webkit-transform: rotate(-45deg) translate(-9px, 6px);
        transform: rotate(-45deg) translate(-9px, 6px);
    }

    .change .bar2 {opacity: 0;}

    .change .bar3 {
        -webkit-transform: rotate(45deg) translate(-8px, -8px);
        transform: rotate(45deg) translate(-8px, -8px);
    }
    a{
        text-decoration: none;
        color: #111;
    }
    .header{
        width: 100%;
        display: flex;
        flex-direction: row;
        font-family: 'Roboto Condensed', sans-serif;
        box-shadow: 0 5px 5px rgba(0, 0, 0, 0.5);
        margin-bottom: 5px;
        align-items: center;
    }
    .logo {
        display: flex;
        flex-direction: row;
        align-items: center;
        height: 100%;
    }
    .navbar {
        height: 100%;
        display: flex;
        align-items: center;
        margin-left: auto;
    }
    .navbar img{
        width: 25px;
        height: 25px;
        vertical-align: middle;
    }
    .home:hover{
        cursor: pointer;
    }
    .navbar a {
        text-decoration: none;
        color: black;
        font-family: 'Roboto Condensed', sans-serif;
        text-transform: uppercase;
        vertical-align: middle;
        transition: ease-out 0.5s;
    }
    .navbar a.active{
        text-decoration: underline;
        font-weight: bold;
        color:#E91E63;
    }
    .navbar a:hover {
        color:#E91E63;
        transition: ease-in 0.5s;
        transform: translateY(-5px);
    }

        /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .header {
        height: 50px;
        }
        .logo{
            margin-left: 10px;
        }   
        .logo img{
            width: 40px;
            height: 40px;
        }
        .logo p{
            margin-left: 10px;
            font-size: 1.5em;
        }
        .navbar {
            margin-right: 0px;
        }
        .navbar img{
            width: 20px;
            height: 20px;
            vertical-align: middle;
        }
        .navbar a {
            font-size: 0.7em;
            text-transform: uppercase;
            margin-left: 10px;
            transition: ease-out 0.5s;
        }
        .navbar-link {
            display: none;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 600px) {
        .header {
            height: 50px;
        }
        .logo{
            margin-left: 10px;
        }   
        .logo img{
            width: 40px;
            height: 40px;
        }
        .logo p{
            margin-left: 10px;
            font-size: 1.5em;
        }
        .navbar {
            margin-right: 0px;
        }
        .navbar img{
            width: 20px;
            height: 20px;
            vertical-align: middle;
        }
        .navbar a {
            font-size: 0.7em;
            text-transform: uppercase;
            margin-left: 10px;
            transition: ease-out 0.5s;
        }
        .navbar-link {
            display: none;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) {
        .header {
            height: 70px;
        }
        .logo{
            margin-left: 10px;
        }   
        .logo img{
            width: 40px;
            height: 40px;
        }
        .logo p{
            margin-left: 10px;
            font-size: 1.5em;
        }
        .navbar {
            margin-right: 20px;
        }
        .navbar img{
            width: 20px;
            height: 20px;
            vertical-align: middle;
        }
        .navbar a {
            font-size: 0.9em;
            text-transform: uppercase;
            margin-left: 15px;
            transition: ease-out 0.5s;
        }
        .main {
            display: none;
        }
        .navbar-link {
            display: inline-block;
        }
    } 

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) {
        .header {
            height: 70px;
        }
        .logo{
            margin-left: 10px;
        }   
        .logo img{
            width: 40px;
            height: 40px;
        }
        .logo p{
            margin-left: 10px;
            font-size: 1.5em;
        }
        .navbar {
            margin-right: 20px;
        }
        .navbar img{
            width: 20px;
            height: 20px;
            vertical-align: middle;
        }
        .navbar a {
            font-size: 1em;
            text-transform: uppercase;
            margin-left: 20px;
            transition: ease-out 0.5s;
        }
        .main {
            display: none;
        }
        .navbar-link {
            display: inline-block;
        }
    } 

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {
        
        .main {
            display: none;
        }
        .navbar-link {
            display: inline-block;
        }
    }

</style>