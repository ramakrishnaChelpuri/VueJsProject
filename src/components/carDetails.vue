<template>
<div class="container">
        
       <h1 class="headline">{{car.car}}</h1>
       <img class="car-image" :src=car.image />
       <div class="green">
       {{car.availability ? 'Available':'Not Avaialble'}}
       </div>
      
      <div class="text">
        <p> Model : {{car.model}}</p>
        <p>Make : {{car.make}}</p>
        <p>Car Type : {{car.car_type}}</p>
        <p>Deposite : {{car.deposit}}$</p>
        <p>Price per Day : {{car.price_per_day}}$</p>
        <p>Insurance Cost : {{car.Insurance}}$</p>
        <p>Tax : {{car.tax}}$</p>
      </div>

</div>
</template>

<script>
    export default {
        name: 'carDetails',
        props: {
            car: Array
        }
    }

</script>

<style>
    .container{
        background-color: #0gfa9f7;
        display:inline-block;
        border:2px solid black;
        padding:10px;
        margin:10px;
        width:550px;
        border-radius:10px;
    }

    .car-image {
        display:flex;
        height: 300px;
        width: 480px;
        border-radius: 10px;
    }


    .headline {
        padding: 3px;
        text-align:center;
    }

    .text{
        text-align:center;
        font-weight:700;
        font-size:1rem;
    }
    
    .green{
        text-align:center;
        font-weight:900;
        color:green;
        padding:10px;
    }
 
</style>