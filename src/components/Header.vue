<script setup>

</script>

<template>
 <header class="header" id="header">
 <nav class="nav container">
 <a href="#" class="nav__logo">
 <i class="bx bxs-watch nav__logo-icon"></i> Rolex
 </a>
 
 <div class="nav__menu" id="nav-menu">
 <ul class="nav__list">
 <li class="nav__item">
 <a href="#home" class="nav__link active-link">Home</a>
 </li>
 <li class="nav__item">
 <a href="#featured" class="nav__link">Featured</a>
 </li>
 <li class="nav__item">
 <a href="#products" class="nav__link">Products</a>
 </li>
 <li class="nav__item">
 <a href="#new" class="nav__link">New</a>
 </li>
 </ul>
 
 <div class="nav__close" id="nav-close">
 <i class="bx bx-x"></i>
 </div>
 </div>

 <div class="nav__btns">
 <i class="bx bx-moon change-theme"></i>

 <div class="nav__shop" id="cart-shop">
 <i class="bx bx-shopping-bag"></i>
 </div>

 <div class="nav__toggle" id="nav-toggle">
 <i class="bx bx-grid-alt"></i>
 
 </div>
 </div>
 </nav>
 
 </header>
</template>

<style scoped>
.header {
    width: 100%;
    background: transparent;
    position: fixed;
    top: 0;
    left: 0;
    z-index: var(--z-fixed);
    /*For animation dark mode*/
    transition: .4s;
}

.nav {
    height: var(--header-height);
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav__logo, 
.nav__toggle,
.nav__shop,.nav__close {
  color: var(--title-color);
}

.nav__logo {
    text-transform: uppercase;
    font-weight: var(--font-bold);
    letter-spacing: 1px;
    display: inline-flex;
    align-items: center;
    column-gap: .25rem;
}

.nav__logo-icon {
    font-size: 1.25rem;
}

.nav__btns {
    display: flex;
    align-items: center;
    column-gap: 1rem;
}

.nav__toggle,
.nav__shop {
    font-size: 1.25rem;
    cursor: pointer;
}

@media screen and (max-width: 767px) {
    .nav__menu {
        position: fixed;
        background-color: var(--body-color);
        top: 0;
        right: -100%;
        width: 100%;
        height: 100%;
        padding: 6rem 2rem 3.5rem;
        transition: .3s;
        }
}

     .nav__list {
        display: flex;
        flex-direction: column;
        align-items: center;
        row-gap: 2rem;
     }

     .nav__link {
        color: var(--title-color);
        font-weight: var(--font-medium);
        text-transform: uppercase;
        font-size: var(--h2-font-size);
        transition: .3s;
     }

     .nav__link:hover {
        color: var(--first-color);
     }

     .nav__close {
        font-size: 2rem;
        position: absolute;
        top: .9rem;
        right: 1.25rem;
        cursor: pointer;
     }

     .show-menu {
        right: 0;
     }

     .scroll-header {
        background-color: var(--first-color-color);
        box-shadow: 0 1px 4px hsla(0, 4%, 15%, .10);
     }

     .active-link {
        color: var(--first-color);
     }

</style>
