<template>
    <section class="work" id="work">
        <div class="wrapper">
            <h2>My work</h2>
            <h3>Previous projects</h3>
            <div class="container-work">
                <div class="container-img">
                    <img alt="hamster-wars" class="work-img" src="@/assets/pre_proj_hamster-wars.png">
                </div>
                <div class="work-desc">
                    <h4>Hamster Wars</h4>
                    <p>Made for a school excercize where we were to build a fullstack app with Node.js and Express.js as the backend. Firestore is used as database.
                        Frontend was built with React and Typescript. For API calls I used Axios.
                    </p>
                    <div class="btn-link-holder">
                        <button class="btn-link"><a href="https://hamsterwars-project-fullstack.herokuapp.com/">View site</a></button>
                        <button class="btn-link"><a href="https://github.com/emiagren/hamsterwars-project">View code</a></button>
                    </div>
                </div>
            </div>
            <div class="container-work">
                <div class="container-img">
                    <img alt="e-wallet" class="work-img" src="@/assets/pre_proj_ewallet.png">
                </div>
                <div class="work-desc">
                    <h4>E-Wallet</h4>
                    <p>Made for a school excercize where we were to build a fullstack app with Node.js and Express.js as the backend. Firestore is used as database.
                        Frontend was built with React and Typescript. For API calls I used Axios.
                    </p>
                    <div class="btn-link-holder">
                        <button class="btn-link"><a href="https://github.com/emiagren/iths-e-wallet">View code</a></button>
                    </div>
                </div>
            </div>
            <div class="container-work">
                <div class="container-img">
                    <img alt="beer-project" class="work-img" src="@/assets/pre_proj_beer_project.png">
                </div>
                <div class="work-desc">
                    <h4>Beer Project</h4>
                    <p>Made for a school excercize where we were to build a fullstack app with Node.js and Express.js as the backend. Firestore is used as database.
                        Frontend was built with React and Typescript. For API calls I used Axios.
                    </p>
                    <div class="btn-link-holder">
                        <button class="btn-link"><a href="https://github.com/HarshadaMulye/beer-project">View code</a></button>
                    </div>
                </div>
            </div>
            <div class="container-work">
                <div class="container-img">
                    <img alt="sinus-webshop" class="work-img" src="@/assets/pre_proj_sinus.png">
                </div>
                <div class="work-desc">
                    <h4>Sinus Webshop</h4>
                    <p>Made for a school excercize where we were to build a fullstack app with Node.js and Express.js as the backend. Firestore is used as database.
                        Frontend was built with React and Typescript. For API calls I used Axios.
                    </p>
                    <div class="btn-link-holder">
                        <button class="btn-link"><a href="https://github.com/annashokhireva/sinus-webshop">View code</a></button>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <div class="bottom-angle"></div>
</template>

<script>

export default {
  name: 'MyWork',
}
</script>

<style scoped>

.work {
    background-color: #aca3be;
    padding: 3rem 1.5rem 3rem;
}

.container-work {
    margin-bottom: 4rem;
}

img {
    display: block;
    width: 100%;
    min-width: 100%
}

.bottom-angle {
    background-color: #aca3be;
    height: 36px;
    width: 100%;
    clip-path: polygon(29% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

@media screen and (min-width: 768px) {

    .container-img {
        width: 55%;
    }

    .work-desc {
        width: 45%;
        margin: 0 3rem; 
    }

    .container-work {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: flex-start;
    }

    .container-work:nth-child(odd) .work-desc {
        order: -1;
    }
}
</style>