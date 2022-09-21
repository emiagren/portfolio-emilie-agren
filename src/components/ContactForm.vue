<template>
    <section class="contact" id="contact">
        <div class="wrapper">
            <h2>Contact</h2>
            <h3>Get in touch</h3>
            <div class="container-contact">
                <div class="container-form">
                <p>
                    At the moment I am looking for any new junior frontend positions, full time or part time. 
                    Do you have an opening for a junior developer or a project where you think I would fit in? 
                    I'd love to hear from you!
                </p>
                <form id="fs-frm" name="simple-contact-form" accept-charset="utf-8" action="https://formspree.io/f/mkneozao" method="post">
                    <label for="full-name">Name<span class="required">*</span></label>
                    <input type="text" name="name" id="full-name" placeholder="Your name" required="">
                    <label for="email-address">Email Address<span class="required">*</span></label>
                    <input type="email" name="_replyto" id="email-address" placeholder="email@example.com" required="">
                    <label for="message">Message<span class="required">*</span></label>
                    <textarea rows="5" name="message" id="message" placeholder="Hi Emilie, you seem nice. Let's collaborate!" required=""></textarea>
                    <input type="hidden" name="_subject" id="email-subject" value="Contact Form Submission">
                <button type="submit" value="Send">Send message</button>
                </form>
                </div>
                <div class="container-social">
                    <p>You can also find me on the following online spaces.</p>
                    <div class="icons-wrapper">
                        <div class="icon">
                            <i class="devicon-linkedin-plain"></i>
                        </div>
                        <div class="icon">
                            <i class="devicon-github-original"></i>
                        </div>
                        <div class="icon">
                            <i class="devicon-facebook-plain"></i>
                        </div>
                        <div class="icon">
                            <img src="@/assets/instagram.svg">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>

export default {
  name: 'ContactForm',
}
</script>

<style scoped>
.contact {
  background-color: #dee1ee;
  padding: 3rem 1.5rem 3rem;
}

form {
    display: block;
}

form label, form input, form textarea {
    width: 100%;
    display: block;
    padding: 1.2rem 0.6rem 0.4rem;
    font-family: 'Poppins', sans-serif;
}

form label {
    font-family: 'Poppins', sans-serif;
}

form input {
    height: 48px;
    border-radius: 4px;
    border: none;
}

form textarea {
    height: 150px;
    border: none;
    border-radius: 4px;
    margin: 0 0 1rem;
}

.required {
    color: red;
}

.container-social {
    margin-top: 1rem;
}

.icons-wrapper {
    margin: 0 0 0.6rem;
    margin-top: 2rem;
}

.icon {
    font-size: 1.6rem;
    color: #343434;
}

@media screen and (min-width: 768px){

.container-contact {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
}

.container-form {
    width: 60%;
}

.container-social {
    width: 30%;
    margin-top: 0;
}

}
</style>