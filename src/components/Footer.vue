<template>
    <footer class="container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-3">
                    <div class="about">
                        <h5>About myPadi</h5>
                        <p>myPadi is an online off-campus hostel renting service for students & NYSC members in Nigeria</p>
                    </div>
                </div>
                <div class="col-md-3">
                    <div class="company">
                        <h5>Company</h5>
                        <ul>
                            <li><router-link to="/blog" class="footer__links">Blog</router-link></li>
                            <li><router-link to="/listings" class="footer__links">List A Hostel</router-link></li>
                            <li><router-link to="/blog" class="footer__links">Become an ambassador</router-link></li>
                            <li><router-link to="/blog" class="footer__links">Invite Friends</router-link></li>
                        </ul>
                    </div>
                </div>
                <div class="col-md-3">
                    <div class="help">
                        <h5>Help</h5>
                        <ul>
                            <li><router-link to="/contact" class="footer__links">Contac Us</router-link></li>
                        </ul>
                    </div>
                </div>
                <div class="col-md-3">
                    <div class="find">
                        <h5>Find Hostel In</h5>
                         <ul>
                            <li><router-link to="/contact" class="footer__links">Unilag</router-link></li>
                            <li><router-link to="/contact" class="footer__links">Uniben</router-link></li>
                            <li><router-link to="/contact" class="footer__links">Delsu</router-link></li>
                        </ul>
                    </div>
                </div>
            </div>
            <hr />
            <div class="row pb-3">
                <div class="col-md-4">
                    <p>Copyright &copy; 2019. myPadi.ng. All rights reserved</p>
                </div>
                <div class="col-md-2">
                    <router-link to="/terms" class="bottom__links">Terms</router-link>&nbsp;&nbsp;&nbsp;&nbsp;
                    <router-link to="/privacy-policy" class="bottom__links">Privacy</router-link>
                </div>
                <div class="col-md-4"></div>
                <div class="col-md-2">
                    <i class="fa fa-facebook-f social__link"></i>
                    <i class="fa fa-twitter social__link"></i>
                    <i class="fa fa-instagram social__link"></i>
                </div>
            </div>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'Footer'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
footer{
        font-family: 'Roboto';
    h5{
        color: rgb(85, 85, 85);
        font-weight: bold;
        padding-bottom: .4rem;
        opacity: .7;
    }
    p{
        font-family: 'Roboto';
        font-size: .92rem;
        color:#484848;
        opacity: .7;
    }
    .footer__links{
        color:#484848;
        text-decoration: none;
        font-size: .9rem;
        font-weight: bold;
        opacity: .5;
        &:hover{
            color:$primary-color;
            transition: all ease-out .5s;
        }
    }
    .bottom__links{
        color: rgb(85, 85, 85);
        opacity: .7;
        text-decoration: none;
        font-weight: bold;
        font-size: .9rem;
    }
    .social__link{
        padding-left: 1rem;
        font-weight: bold;
        color: rgb(85, 85, 85);
        opacity: .7;
    }
}
</style>