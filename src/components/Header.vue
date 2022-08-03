<script setup>

</script>

<template>
 <div>
 <div class="nav-menu">
 <i class="fas fa-bars"
 @click="showMenu()"></i>

 <div class="nav-content">
 <div class="logo">LOGO</div>

 <ul class="nav-items">
 <li>Home</li>
 <li>About</li>
 <li>Contact</li>
 </ul>

 <div class="login-button">Login</div>
 </div>
 </div>
 </div>
</template>

<style lang="scss" scoped>
.nav-menu {
    background-color: var(--secondary-color);
}

.nav-content {
    display: flex;
    justify-content: space-between;
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
    padding: 0 10px;
}

i {
    display: none;
}

// Mobile version - hidden hamburger menu
@media screen and (max-width: 768px) {
    .nav-menu {
        padding-top: 10px;
        position: absolute;
        width: 100%;
    }
    .open-menu {
        
    }
}

</style>
