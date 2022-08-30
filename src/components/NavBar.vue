<template>
    <nav>
        <div class="hamburger" @click="showMenu">
            <span class="bar1"></span>
            <span class="bar2"></span>
            <span class="bar3"></span>
        </div>
        <div class="nav-content" :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'">
            <ul class="nav-items">
                <li>Home</li>
                <li>About me</li>
                <li>Skills and tools</li>
                <li>My work</li>
                <li>Contact</li>
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
    },

}

</script>

<style scoped>
nav {
background-color: #ff5724;
color: #ffe0d6;
font-family: 'Poppins';
font-size: 1.2rem;
position: sticky;
z-index: 99;
opacity: 85%;
top: 0;
left: 0;
right: 0;
}

.nav-content {
padding: 10px 30px;
align-items: center;
}

.nav-items {
display: flex;
justify-content: center;
align-items: center;
list-style: none;
margin: 0;
padding: 0;
}

li {
padding: 0 1.4rem;
}

li:hover {
color: #fff;
}

.hamburger span{
display: none;
}

/* Mobile version - hidden hamburger menu */

    @media screen and (max-width: 768px) {
    nav {
    display: flex;
    flex-direction: column;
    }

    .hamburger {
    padding: 1rem;
    align-self: flex-end;
    }

    .nav-menu {
    padding-top: 10px;
    position: absolute;
    width: 100%;
    }

    .nav-items li{
    padding: 10px;
    }

    .open-menu {
    opacity: 1;
    height: auto;
    }

    .closed-menu {
    opacity: 0;
    height: 0;
    padding: 0;
    }

    .nav-content {
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
    background-color: #FFB198;
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