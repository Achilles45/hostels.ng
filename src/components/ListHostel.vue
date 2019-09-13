<template>
    <section class="list">
        <div class="container">
            <div class="row text-center">
                <div class="col-md-3"></div>
                <div class="col-md-6">
                    <img src="../assets/chair.png" class="img-fluid chair" alt="">
                    <h4>Do you have hostels for rent?</h4>
                    <p>Let's give you your student tenant now!</p>
                    <router-link to="/login" class="listing__btn">Start Listing Now</router-link>
                </div>
                <div class="col-md-3"></div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name:'List'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.list{
    background: url('../assets/banner2.png');
    background-size: cover;
    background-position:center;
    background-repeat: no-repeat;
    padding: 5rem 0;
    color:#fff;
    margin-bottom: 4rem;
    font-family: 'Roboto';
    .chair{
        height: 120px;
        padding-bottom: 1.2rem;
    }
    h4{
        font-size: 2.2rem;
        font-weight: 400;
        letter-spacing: .5px;
    }
    p{
        padding-bottom: 2rem;
    }
    .listing__btn{
        background: $primary-color;
        color:#fff;
        padding: .75rem 2rem;
        text-decoration: none;
    }
}
</style>