<template>
    <section class="ambassador">
       <div class="container">
           <div class="row">
               <div class="col-md-4 pb-4">
                   <img src="../assets/ambassador.jpg" class="img-fluid" alt="">
               </div>
               <div class="col-md-5">
                   <h4>You can make ₦20,000 weekly as myPadi Ambassador</h4>
                   <p>Submitting hostels from landlords near your campus</p>
                   <router-link to="/ambassador" class="ambassador__btn">Find Out More</router-link>
               </div>
               <div class="col-md-3"></div>
           </div>
       </div>
    </section>
</template>
<script>
export default {
    name: 'Ambassador'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.ambassador{
    font-family: 'Roboto';
    margin: 4rem 0;
    h4{
        font-weight: bold;
        color: rgb(72, 72, 72);
    }
    p{
        color: rgb(72, 72, 72);
        font-size: .96rem;
        padding-bottom: .5rem;
    }
    .ambassador__btn{
        background: $primary-color;
        color:#fff;
        text-decoration: none;
        padding: .7rem 1rem;
        font-size: .95rem;
    }
}
</style>