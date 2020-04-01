<template>
    <div class="footer">
        <img src="../../assets/img/icons_hololens.svg" alt="">
        <p>&copy;2020 - HRCAR TEAM хөгжүүлэв. V2.2.0</p>
    </div>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="css" scoped>
    .footer{
        height: 40px;
        background: #34495E;
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .footer img {
        height: 30px;
        margin-left: 10px;
    }
    .footer p {
        color: #ffffff;
        font-family: 'Roboto Condensed', sans-serif;
        margin: auto;
        font-size: 0.9em;
    }
</style>