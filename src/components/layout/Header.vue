<template>
    <div class="header">
        <a href="/">
            <div class="logo">
            <img src="../../assets/logo/ar.svg" alt="">
            <p>Augmented Reality</p>
        </div>
        </a>
        <div class="navbar">
            <span class="home">
                <img src="../../assets/img/icons8-augmented-reality-64.png">
                <router-link to="/" >НҮҮР</router-link>
            </span>
            <router-link to="/Assignment">Бие даалт</router-link>
            <router-link to="/About">Бидний тухай</router-link>
            <router-link to="/Contact">Холбоо барих</router-link>
        </div>
    </div>
</template>

<script>

export default {
    name: "Header"
}
</script>

<style lang="css" scoped>
    a{
        text-decoration: none;
        color: #111;
    }
    .header{
        width: 100%;
        height: 70px;
        background: #ffffff;
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
        margin-left: 20px;
        align-items: center;
        height: 100%;
    }
    .logo img{
        width: 50px;
        height: 50px;
    }
    .logo p{
        margin-left: 10px;
        font-size: 1.5em;
    }
    .navbar {
        height: 100%;
        display: flex;
        align-items: center;
        margin-left: auto;
        margin-right: 30px;
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
        font-size: 1em;
        text-transform: uppercase;
        margin-left: 20px;
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

</style>