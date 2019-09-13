<template>
    <section class="process container-fluid">
        <div class="container">
            <div class="row text-center">
               <div class="col-md-1"></div>
               <div class="col-md-10">
                    <div class="process__heading">
                    <h4>Built for students & NYSC members</h4>
                    <p>We know how hard it can be to find housing as a student or NYSC member, so we created myPadi.ng to make a better process for students and landlords.</p>
                    <a href="#">Read testimonies from some of them &nbsp; <i class="fa fa-long-arrow-right"></i></a>
                </div>
               </div>
             <div class="col-md-1"></div>
            </div>
            <div class="process__wrapper">
                <div class="process__card text-center">
                    <i class="fa fa-check-circle process-icons"></i>
                    <h4>See Verified Listings</h4>
                    <p>We have verified listings from verified landlords in the 60+ cities we operate in. We carefully handpick each of them through of expert network of local housing consultants</p>
                </div>
                <div class="process__card text-center">
                    <i class="fa fa-search process-icons"></i>
                    <h4>Easy searching & renting</h4>
                    <p>Everything is done in one seamless experience; browsing areas, finding directions & distance to school or PPA, and booking and paying for the space. All of this happens in minutes.</p>
                </div>
                <div class="process__card text-center">
                    <i class="fa fa-comments process-icons"></i>
                    <h4>24/7 Support</h4>
                    <p>We're always available & active on Social Media, Phone and email all round the clock. We'll always hold you hand in hand.</p>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'Process'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.process{
    background: url('../assets/map.jpg');
    box-shadow: inset 0 0 0 1000px rgba(0,0,0,.01);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    padding: 4rem 0;
    .process__heading{
        font-family: 'Roboto';
        color: rgb(85, 85, 85);
        h4{
            font-weight: 600;
            font-size: 1.8rem;
        }
        p{
            font-size: 1.1rem;
        }
        a{
            color:$primary-color;
            font-weight: bold;
            font-size: 1rem;
        }
    }
    .process__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 20px;
        font-family: 'Roboto';
        padding-top: 4rem;
       .process-icons{
           color:$primary-color;
           font-size: 3rem;
       }
       h4{
            font-weight: 600;
            color: rgb(85, 85, 85);
            font-size: 1.2rem;
            padding-bottom: .2rem;
            padding-top: .1rem;
       }
       p{
           font-size: .95rem;
            color: #484848;
       }
    }
}
</style>