<template>
   <div class="wrap">
        <div class="card" >
            <div class="card_img">
                <nuxt-link to="`/books/adventure/${data.id}`">
                <img :src='image' alt="">  
                </nuxt-link>
            </div>
            <div class='card_text'>
                <h3 class='title'>{{name}}</h3>
                <p class='description'>{{description}}</p>
                <p class='price'>{{price}} Euro</p>
            </div>
        </div>
   </div>
</template>

<script>
export default {

 props: ['image', 'name', 'description','price','route'],
}
</script>

<style scoped lang='scss'>
.wrap {
    padding: 1rem;
    border: 1px solid black;
    width:80%;
}
 .card{
     display:flex;
     flex-direction:row;
     padding:1rem;
     width:80%;
    }
 .card_img {
     flex-basis: 320px;
  
 }
 .card_text {
    width:50%; 
    display:flex;
    flex-direction:column;
    justify-content: space-evenly;
    .title {
        font-size:3rem;
    }
    .price {
        font-size:1.5rem;
    }
 }
</style>