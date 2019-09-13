<template>
    <section class="home__hostels">
        <div class="home__hostels__text">
            <h3>In which school do you need an accommodation?</h3>
            <p>Discover & rent the best off-campus accommodations around your school easily</p>
        </div>
        <div class="container">
        <div class="row mt-5">
        <div @click="getDetails()" class="col-md-4 hostel__wrapper" v-for="(data, index) in hostels" :key="index">
             <img :src="data.image" class="img-fluid hostel__img" alt="">
             <div class="hostel__details d-flex justify-content-between">
                 <div class="title">
                    <h6>{{ data.school }}</h6>
                    <p>{{data.name }}</p>
                 </div>
                <div class="price">
                    <h6>{{ data.price }}</h6>
                    <p>Verified</p>
                </div>
             </div>
        </div>
        </div>
        </div>
        <!-- <div>
            {{ hostels }}
        </div> -->
    </section>
</template>
<script>
import axios from 'axios';
export default {
    name:'HomeHostels',
    data(){
        return{
            hostels:[
                 {
                    id: 1,
                    name:'Merrytime Hostel',
                    description: "Merytime Hostel is a modern block of student accomodation in Delta State University, Abraka. It is located along winner's road, Abraka. It is just 15mins walk from campus three. It is close to all the facilities to make you comfortable, from market, banks, pharmacy shops, to churches.",
                    image: require('../assets/hostel1.jpg'),
                    price: '100k per year',
                    type: 'Mixed Hostel',
                    location: "10 Winner's road, Abraka",
                    school:"Delta State University, DELSU"
                },
                 {
                    id: 1,
                    name:'Odumegu Hostel',
                    description: "Merytime Hostel is a modern block of student accomodation in Delta State University, Abraka. It is located along winner's road, Abraka. It is just 15mins walk from campus three. It is close to all the facilities to make you comfortable, from market, banks, pharmacy shops, to churches.",
                    image: require('../assets/hostel2.jpg'),
                    price: '100k per year',
                    type: 'Mixed Hostel',
                    location: "College Road, Nnsukka",
                    school:"University of Nigeria UNN"
                },
                 {
                     id: 1,
                    name:'Open view Hostel',
                    description: "Merytime Hostel is a modern block of student accomodation in Delta State University, Abraka. It is located along winner's road, Abraka. It is just 15mins walk from campus three. It is close to all the facilities to make you comfortable, from market, banks, pharmacy shops, to churches.",
                    image: require('../assets/hostel10.jpg'),
                    price: '120k per year',
                    type: 'Mixed Hostel',
                    location: "12 XYZ Street, Yaba.",
                    school:"University of Lagos UNILAG"
                }
            ]
        }
    },
    methods:{
        getDetails:function(){
            alert('Coming soon ...');
        }
    }
//    mounted(){
//        axios
//       .get('home-hostels.json')
//       .then((response)=>{
//           this.hostels = response.data.hostels
//           console.log(this.hostels.name)
//       })
//    }
}
</script>
<style lang="scss" scoped>
.home__hostels{
    .home__hostels__text{
        padding-left: 1rem;
        font-family: 'Roboto';
        h3{
            font-weight: bold;
            color: rgb(85, 85, 85) !important;
            opacity: .8;
            font-size: 1.5rem;
        }
        p{
            color: rgb(85, 85, 85);
        }
    }
}
.hostel__wrapper{
    margin-bottom: 3rem;
    cursor: pointer;
    .hostel__img{
        border-radius: 3px; 
        width: 100% !important;
    }
    .hostel__details{
        padding: .7rem .6rem;
        box-shadow: 0px 0px 3px rgba(0,0,0,.30);
        font-family: 'Roboto';
        border-bottom-left-radius: 3px;
        border-bottom-right-radius: 3px;
        h6{
            color:#484848;
            font-weight: bold;
            font-size: .95rem;
        }
        p{
            color:#484848;
            font-size: .9rem;
        }
    }
}

//MEDIA QUERIES
@media screen and (max-width: 768px){
    .home__hostels__text{
        h3{
            font-size: 1.5rem;
            font-weight: normal;
            line-height: 1.5;
        }
    }
}
</style>