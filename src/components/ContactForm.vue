<template>
    <section class="contact" id="contact">
        <div class="wrapper">
            <h2>Contact</h2>
            <h3>Get in touch</h3>
            <div class="container-contact">
                <div class="container-form">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac lobortis ante, vel pellentesque metus. Maecenas eu aliquet felis.</p>
                <form id="fs-frm" name="simple-contact-form" accept-charset="utf-8" action="https://formspree.io/f/mkneozao" method="post">
                    <label for="full-name">Full Name<span class="required">*</span></label>
                    <input type="text" name="name" id="full-name" placeholder="First and Last" required="">
                    <label for="email-address">Email Address<span class="required">*</span></label>
                    <input type="email" name="_replyto" id="email-address" placeholder="email@domain.tld" required="">
                    <label for="message">Message<span class="required">*</span></label>
                    <textarea rows="5" name="message" id="message" placeholder="Hi Emilie, you seem nice. Let's collaborate!" required=""></textarea>
                    <input type="hidden" name="_subject" id="email-subject" value="Contact Form Submission">
                <button type="submit" value="Send">Send message</button>
                </form>
                </div>
                <div class="container-social">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac lobortis ante, vel pellentesque metus. Maecenas eu aliquet felis.</p>
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
  background-color: #F1EAFF;
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

label {
    font-family: 'Poppins', sans-serif;
}

input {
    height: 48px;
    border-radius: 4px;
    border: none;
}

textarea {
    height: 150px;
    border: none;
    border-radius: 4px;
    margin: 0 0 1rem;
}

.required {
    color: red;
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
}

}
</style>