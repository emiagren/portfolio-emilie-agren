<template>
  <section class="about" id="about">
      <div class="wrapper">
          <h2>About me</h2>
          <h3>Long story short</h3>
          <div class="container-about">
            <div class="profile-img">
                <img alt="profile-img" src="@/assets/emilie_vector.svg">
            </div>
            <div class="profile-txt">
              <h4>I am an open-minded and creative person who naturally sets a high standard for what I do.</h4>
              <p>For as long as I can remember I have had an eye for the visual. When I wanted to focus on something new two years ago, I chose Frontend Developer, something that I am very happy with today that I chose.
              Whoever hires me gets an adaptable and loyal colleague who enjoys working in a team as well as independently.
              I look forward to putting my newly acquired skills to the test in a rapidly growing industry with seemingly endless opportunities.</p>
              <p>Sincerely,</p>
              <p>Emilie</p>
            </div>
        </div>       
      </div>
    </section>
    <div class="bottom-angle"></div>
</template>

<script>

export default {
  name: 'AboutMe',
}
</script>

<style scoped>

.about {
  background-color: #C1BBBF;
  padding: 2rem 1.8rem 2rem;
}

.about h4 {
  color: #fff;
}

.about .profile-img {
  max-width: 300px;
}

.about .profile-img {
  /* border-radius: 50%; */
  overflow: hidden;
  margin: 0 auto;
}

img {
  display: block;
  width: 100%;
  min-width: 100%;
}

.bottom-angle {
    background-color: #C1BBBF;
    height: 36px;
    width: 100%;
    clip-path: polygon(29% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

  @media screen and (min-width: 768px){

    .about .profile-img {
      width: 30%;
    }

    .about .profile-txt {
      width: 70%;
      padding-left: 5%;
    }

    .container-about {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
    }

  }
</style>