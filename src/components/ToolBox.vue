<template>
    <section class="toolbox" id="toolbox">
        <div class="wrapper">
            <h2>My skills</h2>
            <h3>Toolbox</h3>
            <p>
                These are the tools and technologies I have skills in or have some experience of so far.
                Humbly I'd say I am most familiar with working with Html, CSS and Javascript in React and Vue but I also
                spent a few fun weeks working in Umbraco for one of my internships.
            </p>
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
                    <i class="devicon-php-plain"></i>
                    <p>PHP</p>
                </div>
                <div class="icon">
                    <i class="devicon-csharp-plain"></i>
                    <p>C#</p>
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
                    <img src="@/assets/umbraco.svg">
                    <p>Umbraco</p>
                </div>
                <div class="icon">
                    <i class="devicon-visualstudio-plain"></i>
                    <p>Visual Studio</p>
                </div>
                <div class="icon">
                    <i class="devicon-figma-plain"></i>
                    <p>Figma</p>
                </div>
                <div class="icon">
                    <i class="devicon-github-original"></i>
                    <p>GitHub</p>
                </div>
                <div class="icon">
                    <i class="devicon-npm-original-wordmark"></i>
                    <p>npm</p>
                </div>
                <div class="icon">
                    <i class="devicon-nodejs-plain-wordmark"></i>
                    <p>Node</p>
                </div>
                <div class="icon">
                    <i class="devicon-sqlite-plain"></i>
                    <p>SQLite</p>
                </div>
                <div class="icon">
                    <img src="@/assets/responsive.svg">
                    <p>Responsive design</p>
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
  background-color: #dee0ee;
  padding: 48px 24px 48px;
}

.bottom-angle {
    background-color: #dee0ee;
    height: 36px;
    width: 100%;
    clip-path: polygon(69% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

.icons-wrapper {
    margin: 0 0 1.6rem;
}

.icon {
    font-size: 72px;
    margin: 1.6rem 1rem 0.6rem;
    color: #38927d;
}

.icon p{
    font-size: 1rem;
}

</style>