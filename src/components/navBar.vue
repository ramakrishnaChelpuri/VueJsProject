<template>
  <div class="navbar">
      <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"> 
      <label>Car Rental Service</label>
  </div>
</template>

<script>

export default {
    name: 'navBar'
}
</script>

<style>
    .navbar {
        font-family: 'Footlight MT';
        font-weight:800;
        display: Grid;
        background-color: #3d77f6;
        color: black;
        height: 5rem;
        padding: 0.2rem;
        margin: 10px;
    }

    .navbar label {
        display: Grid;
        padding: 0.6rem;
        font-size: 4rem;
        margin-bottom: 10px;
        text-align: center;
    }
</style>