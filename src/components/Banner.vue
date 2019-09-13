<template>
    <section class="banner__wrapper mb-4">
        <div class="container">
            <div class="navbar__wrapper">
                <div class="navbar__contents d-flex justify-content-between">
                    <div class="navbar__logo">
                        <h3><router-link to="/" class="logo">Hostels.ng</router-link></h3>
                    </div>
                    <ul class="navbar__items d-flex justify-content-between">
                        <li><router-link to="/" class="nav__link">List A Hostel</router-link></li>
                        <li><router-link to="/" class="nav__link">Make &#8358;20,000</router-link></li>
                        <li><router-link to="/" class="nav__link register">Register</router-link></li>
                        <li><router-link to="/" class="nav__link login">Login</router-link></li>
                    </ul>
                    <div @click="openNav()" class="navbar__toggler d-none">
                        <i class="fa fa-bars"></i>
                    </div>
                </div>
            </div>
            <!--Banner text
            ================-->
            <div class="row banner__text">
                <div class="col-md-2"></div>
                <div class="col-md-8 col-sm-12 col-xs-12">
                    <h2>Find & Rent the best off-campus hostel quickly</h2>
                    <div class="form__wrapper">
                        <form action="" class="d-flex justify-content-beween">
                            <i class="fa fa-search"></i>
                            <input type="text" class="form-control" placeholder="Type in School, City or Area">
                        </form>
                    </div>
                     <h6 class="text-light form__bottom-text">Or Call/WhatsApp 08103515205</h6>
                </div>
                <div class="col-md-2"></div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'Banner',
    methods:{
        openNav:function(){
            const nav = document.querySelector('.navbar__items');
            nav.classList.toggle('open__nav');
        }
    }
}
</script>
<style lang="scss" scoped>

//Banner wrapper
.banner__wrapper{
    background: url('../assets/banner.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    box-shadow: inset 0 0 0 1000px rgba(0,0,0,.5);
    position: relative;

    //Navbar contents
    .navbar__contents{
        font-family: 'Roboto' !important;
        padding-top: 1.9rem;
        .logo{
            color:#fff;
            text-decoration: none;
            font-size: 1.4rem;
            font-weight: bold;
        }
        .navbar__items{
            padding-top: .55rem !important;
            .nav__link{
                color: #fff;
                font-family: 'Roboto' !important;
                font-size: .95rem;
                letter-spacing: .1px;
                text-decoration: none;
                margin-left: 2rem;
            }
            .register, .login{
                border: 1px solid #fff;
                padding: .75rem 2rem;
                border-radius: 2px;
                &:hover{
                    background: #fff;
                    color:#484848;
                    transition: all ease-in-out .5s;
                }
            }
        }
    }
    
}


//Banner Text
.banner__text{
    font-family: 'Roboto';
    padding-top: 12rem;
    padding-bottom: 4rem;
    h2{
        color:#fff;
        font-weight: bold;
        font-family: 'Lato' !important;
        padding-bottom: .2rem;
        // text-shadow: 0.03em 0.03em 0.05em rgba(0,0,0,.17);
    }
    .form__wrapper{
        background: #fff;
        padding: .65rem 0;
        border-radius: 4px;
        form{
            input[type=text]{
                background: transparent;
                border:none;
                box-shadow: none;
                &::placeholder{
                    font-weight: bold;
                    font-size: 1.1rem;
                }
            }
            .fa-search{
                font-size: 1.7rem;
                padding-left: 1.8rem;
                padding-top: .3rem;
                padding-right: 1rem;
            }
        }
    }
    .form__bottom-text{
        font-size: 1.3rem;
        padding-top: 2.5rem;
    }
}

//MEDIA QUERIES
@media screen and (max-width: 990px) {
    .navbar__items{
        background: #484848;
        flex-direction: column;
        position: absolute;
        right: 5%;
        padding: 3rem;
        border-radius: 4px;
        top: 20%;
        display: none !important;
        // height: calc(50vh);
        z-index: 2;
        .nav__link{
            margin-left: 0 !important;
            line-height: 2.9;
        }
        .register, .login{
            border:none !important;
            padding:0 !important;
            &:hover{
                background: transparent !important;
            }
        }
    }
    .navbar__toggler{
        display: block !important;
        font-size: 2rem;
        color:#fff;
        padding-right: 1.5rem;
        cursor: pointer;
    }

    .open__nav{
        display: block !important;
        transition: all ease-in-out .5s;
    }
    //Banner Text
    .banner__text{
        padding-top: 8rem;
        padding-bottom: 3rem;
        h2{
            font-size: 1.7rem;
        }
          .form__bottom-text{
              padding-top: 1.8rem;
          }
    }
}

@media screen and (max-width: 768px){
    .banner__text h2{
        font-size: 1.3rem;
    }
    .navbar__toggler{
        font-size: 1.7rem;
    }
}
</style>