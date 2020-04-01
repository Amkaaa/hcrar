<template>
    <div class="header">
        <a href="/">
            <div class="logo">
            <img src="../../assets/logo/ar.svg" alt="">
            <p>Augmented Reality</p>
        </div>
        </a>
        <div class="navbar">

            <input class="menu-btn" type="checkbox" id="menu-btn" />
            <label class="menu-icon" for="menu-btn"><span class="nav-icon"></span></label>

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

    .navbar .navbar-link {
        max-height: 0;
        transition: max-height .2s ease-out;
    }
    
    #menu-btn:checked ~ .navbar-link {
        right: 0;
    }

    .navbar .menu-icon {
        cursor: pointer;
        float: right;
        padding: 28px 20px;
        position: relative;
        user-select: none;
        margin-right: 20px;
    }

    .navbar .menu-icon .nav-icon {
        background: #333;
        display: block;
        height: 2px;
        position: fixed;
        z-index: 100;
        transition: background .2s ease-out;
        width: 18px;
    }

    .navbar .menu-icon .nav-icon:before,
    .navbar .menu-icon .nav-icon:after {
        background: #333;
        content: '';
        display: block;
        height: 100%;
        position: absolute;
        transition: all .2s ease-out;
        width: 100%;
    }
    .navbar .menu-icon .nav-icon:before {
        top: 5px;
    }

    .navbar .menu-icon .nav-icon:after {
        top: -5px;
    }

    /* menu btn */

    .navbar .menu-btn {
        display: none;
    }

    .navbar .menu-btn:checked ~ .navbar-link {
        max-height: 100vh;
    }

    .navbar .menu-btn:checked ~ .menu-icon .nav-icon {
        background: transparent;
    }

    .navbar .menu-btn:checked ~ .menu-icon .nav-icon:before {
        transform: rotate(-45deg);
        background: #FFFFFF;
        top:0;
    }

    .navbar .menu-btn:checked ~ .menu-icon .nav-icon:after {
        transform: rotate(45deg);
        background: #FFFFFF;
        top:0;
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
    .navbar .navbar-link {
        overflow: hidden;
    }
    .navbar img{
        width: 25px;
        height: 25px;
        vertical-align: middle;
    }
    .navbar .home:hover{
        cursor: pointer;
        transition: ease-in 0.5s;
        transform: translateY(-5px);
    }
    .navbar .navbar-link a{
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
            position: fixed;
            width: 50%;
            height: 100vh;
            background: rgba(0, 0, 0, 0.8);
            right: -100%;
            top: 0;
            text-align: center;
            padding: 80px 0;
            line-height: 2.5;
            transition: 0.7s;
            display: flex;
            flex-direction: column;
            z-index: 10;
        }
        .navbar a {
            color: #FFFFFF !important;
            font-size: 1.5em;
            margin: 0;
        }
        .navbar a.active{
            color:#E91E63 !important;
        }
        .home:hover,
        .navbar a:hover{
            color: #E91E63 !important;
            background: rgba(0, 0, 0, 0.5);
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
            position: fixed;
            width: 50%;
            height: 100vh;
            background: rgba(0, 0, 0, 0.8);
            right: -100%;
            top: 0;
            text-align: center;
            padding: 80px 0;
            line-height: 2.5;
            transition: 0.7s;
            display: flex;
            flex-direction: column;
            z-index: 10;
        }
        .navbar a {
            color: #FFFFFF !important;
            font-size: 1.5em;
            margin: 0;
        }
        .navbar a.active{
            color:#E91E63 !important;
        }
        .home:hover,
        .navbar a:hover{
            color: #E91E63 !important;
            background: rgba(0, 0, 0, 0.5);
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
        .navbar .navbar-link {
            clear: none;
            float: right;
            max-height: none;
        }
        .navbar-link {
            display: inline-block;
        }
        .navbar .menu-icon {
            display: none;
        }
        .navbar-link {
            position: relative;
            width: 100%;
            height: 40px;
            background: #FFFFFF;
            right: 0;
            top: 0;
            text-align: center;
            padding: 0;
            line-height: 2.5;
            transition: 0.7s;
            display: block;
            z-index: 10;
        }
        .navbar a {
            color: #000 !important;
            font-size: 1em;
            margin-left: 10px;
        }
        .navbar a.active{
            color:#E91E63 !important;
        }
        .home:hover,
        .navbar a:hover{
            color: #E91E63 !important;
            background: #FFFFFF;
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
        .navbar .navbar-link {
            clear: none;
            float: right;
            max-height: none;
        }
        .navbar-link {
            display: inline-block;
        }
    } 

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {
        
        .navbar-link {
            display: inline-block;
        }
        .navbar .navbar-link {
            clear: none;
            float: right;
            max-height: none;
        }
        .navbar-link {
            display: inline-block;
        }
    }

</style>