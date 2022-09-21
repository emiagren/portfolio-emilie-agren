<template>
    <nav>
        <div class="nav-content">
            <div class="avatar">
                <img src="../assets/profile_img_emilie.jpg" alt="avatar">
                <!-- <span>emilie ågren</span> -->
            </div>
            <div class="hamburger" @click="showMenu">
                <span class="bar1"></span>
                <span class="bar2"></span>
                <span class="bar3"></span>
            </div>
        </div>
        <div class="nav-list" :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'">
            <ul class="nav-items">
                <li><a :href="href" @click.prevent="scrollTo('#home')">Home</a></li>
                <li><a :href="href" @click.prevent="scrollTo('#about')">About me</a></li>
                <li><a :href="href" @click.prevent="scrollTo('#toolbox')">Skills and tools</a></li>
                <li><a :href="href" @click.prevent="scrollTo('#work')">Projects</a></li>
                <li><a :href="href" @click.prevent="scrollTo('#contact')">Contact</a></li>
            </ul>
        </div>
    </nav>
</template>

<script>

export default {

  name: 'NavBar',

    data() {
        return {
        showMobileMenu: false,
        };
    },

    methods: {
    showMenu() {
        this.showMobileMenu = !this.showMobileMenu;
    },

    scrollTo(selector) {
        document.querySelector(selector).scrollIntoView({ behavior: 'smooth' });
        this.showMobileMenu = false;
    }
}

}

</script>

<style scoped>
nav {
    display: flex;
    justify-content: space-between;
    background-color: #dfd5db;
    font-family: 'Poppins';
    font-size: 1.2rem;
    position: fixed;
    z-index: 10;
    opacity: 90%;
    top: 0;
    left: 0;
    right: 0;
}

nav .avatar {
    display: flex;
    flex-direction: row;
}

nav .avatar img {
    border-radius: 50%;
    margin: 1rem 1rem 1rem 2rem;
    overflow: hidden;
    width: 3rem;
}

nav .avatar span {
    letter-spacing: 0.2rem;
    padding-top: 1.7rem;
    color: #8f7053;
}

.nav-list {
    padding: 1.5rem;
    margin-left: -1.9rem;
}

.nav-items {
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
}

li {
    padding: 0 1.4rem;
}

a {
    color: #8f7053;
    letter-spacing: 0.2rem;
}

li:hover {
    color: #fff;
}

.hamburger span{
    display: none;
}

/* Mobile version - hidden hamburger menu */

    @media screen and (max-width: 1110px) {
    nav {
        display: flex;
        flex-direction: column;
    }

    .nav-content {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .hamburger {
        padding: 1rem;
        margin-right: 1rem;
        align-self: flex-end;
    }

    .nav-menu {
        padding-top: 1rem;
        position: absolute;
        width: 100%;
    }

    .nav-items li{
        padding: 1rem;
    }

    .open-menu {
        opacity: 1;
        height: 100vh;
    }

    .closed-menu {
        opacity: 0;
        height: 0;
        padding: 0;
    }

    .nav-list {
        flex-direction: column;
        z-index: 100;
        position: relative;
        transition: all 0.2s ease-out;
    }

    .nav-items {
        flex-direction: column;
    }

    .hamburger span {
        display: block;
        width: 42px;
        height: 6px;
        margin: 6px auto;
        background-color: #8f7053;
        border-radius: 4px;
        transition: 0.4s;
    }

    .open-menu .hamburger .bar1 {
        transform: rotate(45deg) translate(8px,3px);
    }

    .open-menu .hamburger .bar2 {
        opacity: 0;
    }

    .open-menu .hamburger .bar3 {
        transform: rotate(-45deg) translate(8px,-3px);
    }
}
</style>