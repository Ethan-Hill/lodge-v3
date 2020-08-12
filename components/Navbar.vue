<template>
    <b-navbar class="nav">
        <template slot="brand">
            <b-navbar-item class="navbar-item" tag="router-link" :to="{ path: '/' }">
                <img
                    id="logo"
                    src="../assets/logo.png"
                >
                <h1 id="logo-title">International Lodge</h1>
            </b-navbar-item>
        </template>
        <template slot="start" id="menu">
            <b-navbar-item class="navbar-item" href="/">
                Home
            </b-navbar-item>
            <b-navbar-item class="navbar-item" href="/about">
                About
            </b-navbar-item>
            <b-navbar-item class="navbar-item" href="/staff">
                Staff
            </b-navbar-item>
        </template>

        <template slot="end" id="menu">
            <a style="margin-top:40%; margin-right:50%" href="https://discord.gg/nVHHYQu"><b-button rounded type="is-success">Connect</b-button></a>
        </template>
    </b-navbar>
</template>



<style scoped>

    .nav {
        background-color: #fff;
        color: black;
        min-height: 7vh;
        box-shadow: 0 5px 5px -5px rgba(0,0,0,.4);
    }

    #logo {
        width: 70px;
        min-height: 70px;
        border-radius: 50%;
    }

    #logo-title {
        margin-left: 20px;
        font-weight: bold;
        font-size: 20px;
    }

    #menu {
        display: flex;
        justify-content: center;
        margin-left: 30% !important;
    }

    .navbar-item {
        color: black;
        font-size: 18px;
        margin: 10px;
    }

    .navbar-item:hover {
        transition: 0.5s;
        background: #fff;
        color: black;
        font-size: 18px;
        margin: 10px;
    }
</style>