<script setup lang="ts"></script>

<template>
    <header id="header-container">
        <div class="subcontainer">
            <div class="toggle-content"></div>
            <a href="/" class="header-logo-container">
                <div class="logotipo-container">
                    <img src="/default-logo-md.png" alt="logotipo Gabriel medio">
                </div>
                <div>
                    <h1>Portfólio</h1>
                </div>
            </a>
            <div class="toggle-content"></div>
        </div>
    </header>
</template>

<style scoped>
#header-container {
    width: 100%;
    display: flex;
    justify-content: center;
    position: fixed;
    top: 0;
    z-index: 99;
    backdrop-filter: blur(20px);
}
.subcontainer {
    max-width: 1800px;
    width: 100%;
    display: flex;
    justify-content: center;
    padding: 30px 0;
    position: relative;
}
.subcontainer::after {
    content: "";
    width: 100%;
    height: 1px;
    background-color: var(--purple-background);
    position: absolute;
    bottom: 0;
}
.header-logo-container {
    display: flex;
    align-items: center;
    line-height: 0;
}
.header-logo-container h1 {
    color: white;
    margin: 0;
    font-size: 3.2rem;
}
.logotipo-container img {
    width: 40px;
    margin: 0 5px 0 0;
}
</style>