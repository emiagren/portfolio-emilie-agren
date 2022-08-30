<template>
    <section class="contact">
        <div class="container-contact">
            <h2>Contact</h2>
            <h3>Get in touch</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac lobortis ante, vel pellentesque metus. Maecenas eu aliquet felis.</p>
            <form @submit.prevent="sendMsg">
                <input id="name" type="text" placeholder="Name">
                <input id="email" type="text" placeholder="Email">
                <input id="msg" type="text" placeholder="Message">
                <button>Send message</button>   
            </form>
        </div>
    </section>
</template>

<script>

export default {
  name: 'ContactForm',
}
</script>

<style scoped>
.container-contact {
  background-color: #D9D9D9;
  padding: 50px 25px 50px;
}

.container-contact p{
  margin: 20px 0 16px;
}

form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

input {
    width: 100%;
    height: 32px;
    margin: 16px 8px 8px;
    border-radius: 4px;
    border: none;
    display: inline-block;
}

#msg {
    height: 97px;
}
</style>