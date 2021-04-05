<template>
    <div class="bg-light">
        <div class="container">
            <b-navbar toggleable="lg" type="light" variant="light">
                <b-navbar-nav class="d-block d-sm-none">
                    <b-navbar-brand href="#" class=" position-relative">
                        <img src="../../assets/logo.png" class="position-absolute" alt="logo"
                        srcset="../../assets/logo.png">
                    </b-navbar-brand>
                </b-navbar-nav>
                <b-navbar-toggle target="nav-collapse"
                class="custom-toggler ml-auto"></b-navbar-toggle>

                <b-collapse id="nav-collapse" is-nav class="justify-content-center">
                    <b-navbar-nav class="ml-auto w-12 hide-xs">
                        <b-navbar-brand href="#" class="position-relative">
                            <img src="../../assets/logo.png" class="position-absolute" alt="logo"
                            srcset="../../assets/logo.png">
                        </b-navbar-brand>
                    </b-navbar-nav>
                    <b-navbar-nav>
                        <b-nav-item href="#">Modelos</b-nav-item>
                        <b-nav-item href="#">Prueba de manejo</b-nav-item>
                        <b-nav-item href="#">Cotizar</b-nav-item>
                        <b-nav-item href="#">Promociones</b-nav-item>
                        <b-nav-item href="#">Distribuidores</b-nav-item>
                    </b-navbar-nav>
                    <b-navbar-nav class="ml-auto hide-xs">
                        <b-nav-item href="#">
                            <img src="../../assets/icons/menu.svg" alt="menu"
                            srcset="../../assets/icons/menu.svg">
                        </b-nav-item>
                    </b-navbar-nav>
                </b-collapse>
            </b-navbar>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '../../assets/styles/common';
@import '../../assets/styles/variables';
@import '../../assets/styles/queries';

    .w-12 {
        width: 12.5%;
    }

    .navbar-brand  {
        img {
            margin-top: calc(100% - 36px);
        }
    }

    .navbar-light .navbar-nav .nav-link {
        @extend  %spaced-text;;
        font-weight: 700;
    }

    .custom-toggler.navbar-toggler {
        border-color: rgba(255, 102, 204, 0);
    }
    .navbar-light .navbar-toggler-icon {
        background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='30' height='30' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%280, 0, 255, 0.5%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
    }
</style>
