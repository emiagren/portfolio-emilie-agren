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
                    <p>
                        What do all hamsters have in common? They're ridiculously tiny and cute! But only one can
                        be the cutest right? And that's how the Hamster Wars began... 
                        <br>
                        <br>
                        Made as a school assignment where the purpose was to build a fullstack app. 
                        Node.js and Express.js was used as backend with Firestore as the database.
                        The frontend was built with React and Typescript. For API calls I used Axios.
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
                    <p>
                        This was my first school project working with a framework, in this case Vue. The assignment was to build, 
                        as the name gives away, a simple e-wallet. The task was, in addition to design, to build a form to be able 
                        to add new cards as well as the possibility to delete cards. 
                        <br>
                        <br>
                        This project was never deployed but the code is available to view at GitHub. 
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
                    <p>
                        A Brewdog beer wiki made together with two class mates back in my first term of school. 
                        Built with Html, CSS and Javascript - this was our first go at making a simple website
                        with Javascript and making API calls. 
                        <br>
                        <br>
                        This project was never deployed but the code is available to view at GitHub. 
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
                    <p>
                        A webshop made as a school assignment by me and two class mates. This project was
                        a lot about working agile and for that we used the SCRUM-method. The frontend was built
                        with Vue and the backend was pre coded by our teacher. The goal was for the user to be able
                        to register, login, order and view past orders. For state management we used Vuex.
                        <br>
                        <br>
                        This project was never deployed but the code is available to view at GitHub.  
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
    background-color: #a7a8c2;
    padding: 3rem 1.5rem 3rem;
}

.bottom-angle {
    background-color: #a7a8c2;
    height: 36px;
    width: 100%;
    clip-path: polygon(29% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

.container-work {
    margin-bottom: 4rem;
}

img {
    display: block;
    width: 100%;
    min-width: 100%
}

@media screen and (min-width: 768px) {

    .container-img {
        margin-top: 2rem;
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