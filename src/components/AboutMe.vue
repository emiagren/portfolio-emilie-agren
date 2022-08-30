<template>
  <section class="about">
      <div class="container-about">
        <div class="profile-img-heading">
          <h2>About me</h2>
          <h3>Long story short</h3>
          <div class="profile-img-container">
            <img alt="profile-pic" class="profile-pic" src="@/assets/emilie_profile.jpg">
        </div>
        </div>
        <div class="profile-txt">
          <h4>I am an open-minded and creative person who naturally sets a high standard for what I do.</h4>
          <p>For as long as I can remember I have had an eye for the visual. When I wanted to focus on something new two years ago, I chose Frontend Developer, something that I am very happy with today that I chose.
          Whoever hires me gets an adaptable and loyal colleague who enjoys working in a team as well as independently.
          I look forward to putting my newly acquired skills to the test in a rapidly growing industry with seemingly endless opportunities.</p>
        </div>       
      </div>
      <div class="bottom-angle"></div>
    </section>
</template>

<script>

export default {
  name: 'AboutMe',
}
</script>

<style scoped>
.cloudberry-box {
  background-color: #C3B23B;
}

.cloudberry {
  margin-top: -125px;
  z-index: 2;
}

.container-about {
  background-color: #C3B23B;
  padding: 2rem 1.8rem 2rem;
}

.profile-img-container {
  border-radius: 50%;
  overflow: hidden;
  margin: 0 auto;
}

img {
  display: block;
  width: 100%;
  min-width: 100%;
}

.container-about h3, h4 {
  color: #fff;
}

.container-about p {
  margin-top: 24px;
}

.container-about::before {
    content: url(./../assets/Cloudberry.svg);
    display: block;
    z-index: 1;
    height: auto;
    width: 175px;
    position: absolute;
    margin-top: -98px;
    right: -2px;
}

.bottom-angle {
    background-color: #C3B23B;
    height: 80px;
    width: 100%;
    clip-path: polygon(69% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

  @media screen and (min-width: 600px){
    
    .container-about {
      display: grid;
      grid-template-columns: 50% 50%;
    }

    .profile-img-heading {
      display: flex;
      flex-direction: column;
      padding: 2rem 4rem;
    }

    .profile-txt {
      display: flex;
      flex-direction: column;
      padding: 5rem 4rem;
    }

  }
</style>