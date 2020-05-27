<template>
 <div class="page">
        <Card
        v-for="data in myJson" :key="data.id"
        :image='data.image'
        :name='data.name'
        :description='data.description'
        :price='data.price'
         />
     
    </div>
</template>

<script>
import json from '../../db/database.json';
import Card from '../../components/Card';

export default {
  components: {
    Card 
  },
  props: {
   image: String,
   name: String,
   description:String,
   price:Number
},
     data(){
              return{
                  myJson: json.books.adventure
              }
          }
}
</script>

<style  lang="scss">

</style>