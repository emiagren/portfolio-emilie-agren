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
              <p>
                For as long as I can remember I have had an eye for the visual in an artistic kind of way. As a kid one 
                of my biggest passions were drawing. As a teenager I discovered photo editing and web design. In my 
                twenties I took classes in web design and photography, which were favorite subjects at that point. 
                Through my previous full time job I spiked an interest for IT when doing minor IT works in the coms 
                room and in our offices.
                <br>
                <br>
                So when I wanted to change careers two years ago, I chose Frontend Developer, something that I am very 
                happy today that I chose. One of the things I love most about Frontend developing is that it offers such 
                a broad spectrum of orientations depending on what you like to do and what you’re best at. 
                <br>
                <br>
                Whoever hires me gets an adaptable and loyal colleague who enjoys working in a team as well as independently.
                I look forward to putting my newly acquired skills to the test in a rapidly growing industry with seemingly 
                endless opportunities.
              </p>
              <br>
              <p>Sincerely,</p>
              <br>
              <p class="author-name">Emilie</p>
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
  background-color: #c1c1cf;
  padding: 2rem 1.8rem 2rem;
}

.bottom-angle {
    background-color: #c1c1cf;
    height: 36px;
    width: 100%;
    clip-path: polygon(29% 100%, 100% 38%, 100% 0, 0 0, 0% 38%);
    position: absolute;
}

h4 {
  color: #fff;
}

.profile-img {
  /* border-style: solid;
  border-width: 4px;
  border-color: #fff;
  border-radius: 50%; */
  max-width: 300px;
  overflow: hidden;
  margin: 0 auto;
}

.profile-img img {
  display: block;
  width: 100%;
  min-width: 100%;
}

.author-name {
  font-family: 'La Belle Aurore';
  font-size: 2rem;
}

  @media screen and (min-width: 768px){

    .profile-img {
      margin-top: 2rem;
      width: 30%;
    }

    .profile-txt {
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