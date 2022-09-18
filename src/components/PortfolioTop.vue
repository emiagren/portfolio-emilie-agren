<template>
    <header class="portfolio-top" id="home">
        <div class="intro">
            <div class="title">
                <h1>Hi, I'm Emilie</h1>
                <h2>Frontend Developer</h2>
            </div>
        </div>
        <div class="clouds">
            <img src="../assets/cloud1.png" alt="" style="--i:1">
            <!-- <img src="../assets/cloud2.png" alt="" style="--i:2"> -->
            <img src="../assets/cloud3.png" alt="" style="--i:3">
            <img src="../assets/cloud4.png" alt="" style="--i:4">
            <!-- <img src="../assets/cloud5.png" alt="" style="--i:5"> -->
        </div>
    </header>
</template>

<script>

export default {
  name: 'PortfolioTop',
}
</script>

<style scoped>

.intro {
    background-image: url(./../assets/bg_forest.jpg);
    background-size: cover;
    width: 100%;
    height: 100vh;
    background-position: 70% 30%;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
}

.intro .title {
    font-family: 'Georgia', sans-serif;
}

.intro .title h1 {
    font-size: 5vh;
    color: #ffffff;
    font-family: 'Coromant Garamond', serif;
    letter-spacing: .4rem;
    text-shadow: 1px 1px 2px rgb(116, 116, 116);
}

.intro .title h2 {
    font-size: 2.5vh;
    color: #ffffff;
    text-transform: none;
    margin: 0;
    font-family: 'Coromant Garamond', serif;
    letter-spacing: .4rem;
    text-shadow: 1px 1px 2px rgb(116, 116, 116);
}

.clouds {
    overflow: hidden;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

.clouds img {
    animation: cloud calc(140s * var(--i)) linear infinite;
    opacity: .6;
    position: absolute;
    bottom: 0;

}
@keyframes cloud{
    0%{
        transform: translateX(-20%);
    }
    50%{
        transform: translateX(100%);
    }
}

@media screen and (min-width: 550px) {

    .intro .title h1 {
    font-size: 6.4vh;
    }

    .intro .title h2 {
    font-size: 3.2vh;
    }
}

@media screen and (min-width: 768px) {

    .intro .title h1 {
    font-size: 10vh;
    }

    .intro .title h2 {
    font-size: 5.2vh;
    }
}

</style>