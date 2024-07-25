<template>
    <nav class="navbar">
        <div class="navbar-container">
            <div class="navbar-logo">MyApp</div>
            <ul :class="['navbar-menu', {open: isMenuOpen}]">
                <li class="navbar-item"><router-link to="/" class="navbar-link">Home</router-link></li>
                <li class="navbar-item"><router-link to="/about" class="navbar-link">About</router-link></li>
                <li class="navbar-item"><router-link to="/contact" class="navbar-link">Contact</router-link></li>
            </ul>
            <div class="navbar-toggle" @click="toggleMenu">
                <div class="bar"></div>
                <div class="bar"></div>
                <div class="bar"></div>
            </div>
        </div>
    </nav>
</template>


<script>
    export default {
        name: 'NavbarPage',
        data() {
            return {
                isMenuOpen: false
            };
        },
        methods: {
            toggleMenu() {
                this.isMenuOpen = !this.isMenuOpen;
            }
        }
    };
</script>

<style scoped>
    .navbar {
        background-color: navy;
        color: white;
        padding: 20px 20px;
       position: relative;
    }

    .navbar-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .navbar-logo {
        font-size: 24px;
        font-weight: bold;
    }
    .navbar-menu {
        list-style-type:none;
        margin: 0;
        padding: 0;
        display: flex;
        transition: max-height 0.3s easy-out;
    }
    .navbar-item {
        margin-right: 20px;
    }
    .navbar-link {
        color:white;
        text-decoration: none;
        font-size: 18px;
    }
    .navbar-link:hover{
        text-decoration: aqua;
    }
    .navbar-toggle{
        display: none;
        flex-direction: column;
        cursor: pointer;
    }
    .bar {
        width:25px;
        height:3px;
        background-color: white;
        margin: 4px 0;
    }
    
    @media (max-width: 768px) {
        .navbar-menu {
            display: flex;
            flex-direction: column;
            position: absolute;
            top: 60px;
            left:0;
            width: 100%;
            background-color: navy;
            max-height: 0;
            overflow: hidden;
        }
        .navbar-menu.open {
            /* display:flex; */
            max-height: 200px;
        }
        .navbar-item {
            margin-right: 10px;
            padding-left: 5%;
            margin-bottom: 10px;
            text-align: left;
        }
        .navbar-toggle {
            display: flex;
        }
    }
</style>