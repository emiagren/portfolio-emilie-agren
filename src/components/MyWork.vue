<template>
    <section class="work">
        <div class="container-work">
            <div class="work-img-heading">
                <h2>My work</h2>
                <h3>Previous projects</h3>
                <div class="container-img">
                    <img alt="hamster-wars" class="hamster-wars" src="@/assets/pre_proj_hamster-wars.png">
                </div>
            </div>
            <div class="work-desc">
                <h4>Hamster Wars</h4>
                <p>Made for a school excercize where we were to build a fullstack app with Node.js and Express.js as the backend. Firestore is used as database.
                    Frontend was built with React and Typescript. For API calls I used Axios.
                </p>
                <div class="btn-link-holder">
                    <button class="btn-link"><a href="https://hamsterwars-project-fullstack.herokuapp.com/">View site</a></button>
                    <button class="btn-link"><a href="https://github.com/emiagren/hamsterwars-project">View GitHub</a></button>
                </div>
            </div>
        </div>
        <div class="bottom-angle"></div>
    </section>
</template>

<script>

export default {
  name: 'MyWork',
}
</script>

<style scoped>

.container-work {
  background-color: #FD7C53;
  padding: 48px 24px 48px;
}

.container-work h2 {
    margin-top: 64px;
}

.container-work h3 {
    margin-bottom: 48px;
}

.container-work::before {
    content: url(./../assets/Lingonberries.svg);
    display: block;
    z-index: 1;
    height: auto;
    width: 175px;
    position: absolute;
    margin-top: -124px;
    left: 8px;
    transform: rotate(0.80turn);
}

img {
    display: block;
    width: 100%;
    min-width: 100%
}

.btn-link-holder {
    display: flex;
    justify-content: center;
}

.btn-link {
    margin: 0.6rem;
}

.btn-link a {
    color: #fff;
    text-decoration: none;
}

.bottom-angle {
    background-color: #FD7C53;
    height: 80px;
    width: 100%;
    clip-path: polygon(0 0, 100% 0, 100% 77%, 70% 0, 48% 59%, 26% 16%, 0 76%);
    position: absolute;
}

@media screen and (min-width: 600px){

.container-work {
    display: grid;
    grid-template-columns: 50% 50%;
}

.work-img-heading {
    display: flex;
    flex-direction: column;
    padding: 2rem 4rem;
}

.work-desc {
    display: flex;
    flex-direction: column;
    padding: 5rem 4rem;
}
}
</style>