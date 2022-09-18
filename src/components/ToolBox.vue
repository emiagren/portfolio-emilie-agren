<template>
    <section class="toolbox" id="toolbox">
        <div class="wrapper">
            <h2>Tools & tech</h2>
            <h3>My toolbox</h3>
            <p>These are the tools and technologies I have skills in and would use to bring my projects to life.</p>
            <div class="icons-wrapper">
                <div class="icon">
                    <i class="devicon-html5-plain"></i>
                    <p>HTML5</p>
                </div>
                <div class="icon">
                    <i class="devicon-css3-plain"></i>
                    <p>CSS3</p>
                </div>
                <div class="icon">
                    <i class="devicon-javascript-plain"></i>
                    <p>JavaScript</p>
                </div>
                <div class="icon">
                    <i class="devicon-typescript-plain"></i>
                    <p>TypeScript</p>
                </div>
                <div class="icon">
                    <i class="devicon-react-original"></i>
                    <p>React</p>
                </div>
                <div class="icon">
                    <i class="devicon-vuejs-plain"></i>
                    <p>Vue</p>
                </div>
                <div class="icon">
                    <i class="devicon-wordpress-plain"></i>
                    <p>WordPress</p>
                </div>
                <div class="icon">
                    <i class="devicon-wordpress-plain"></i>
                    <p>Umbraco</p>
                </div>
                <div class="icon">
                    <i class="devicon-github-original"></i>
                    <p>GitHub</p>
                </div>
                <div class="icon">
                    <i class="devicon-figma-plain"></i>
                    <p>Figma</p>
                </div>
            </div>
        </div>
    </section>
    <div class="bottom-angle"></div>
</template>

<script>

export default {
  name: 'ToolBox',
}
</script>

<style scoped>

.toolbox {
  background-color: #F1EAFF;
  padding: 48px 24px 48px;
}

.bottom-angle {
    background-color: #F1EAFF;
    height: 36px;
    width: 100%;
    clip-path: polygon(69% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

.icons-wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 0 0 1.6rem;
}

.icon {
    font-size: 72px;
    padding: 0 0.8rem;
    margin: 1.6rem 1rem 0.6rem;
    text-align: center;
    color: #3FA48C;
}

.icon p{
    font-size: 1rem;
}

</style>