<template>
    <div class="wrapper">
        <div class="top"></div>
        <div class="angles silhouette"></div>    
        <div class="intro">
            <h1>Hi, I'm Emilie</h1>
            <h3>Frontend Developer</h3>
        </div>
        <div class="bottom-angle"></div>
    </div>
</template>

<script>

export default {
  name: 'PortfolioTop',
}
</script>

<style scoped>

.top {
  background-color: #3FA48C;
  height: 200px;
}

.intro {
    background-color: #fff;
    text-align: center;
    font-style: italic;
    color: #276859;
    padding: 48px;
    position: relative;
}

.intro h1 {
    font-size: 6.3vh;
    margin-left: -72px;
}

.intro h3 {
    font-size: 4.2vh;
    margin-right: -72px;
    margin-bottom: 32px;
}

.silhouette{
    background-color: #fff;
    height: 80px;
    width: 100%;
    position: absolute;
    clip-path: polygon(63% 58%, 74% 24%, 100% 100%, 0 100%, 34% 0);
    margin-top: -80px;
}

.bottom-angle {
    background-color: #fff;
    height: 50px;
    width: 100%;
    clip-path: polygon(69% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

@media screen and (min-width: 600px) {
    .intro::after {
        height: 90px;
        transform: skewY(3.4deg);
    }
}

@media screen and (min-width: 600px) {
    .intro::after {
        transform: skewY(3.1deg);
    }
}
</style>