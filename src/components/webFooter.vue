<template>
  <div class="footer">
    <div class="footer-contact">
        Email : car_rentals@gmail.com
    </div>
    <div class="footer-contact">
        Phone : +1 (475) 300 8042
    </div>
    <div class="footer-copyright">
        <span><i class="fa fa-copyright"> Car Rental Services 2022</i></span>
    </div>
  </div>
</template>

<script>

export default {
    name: "webFooter"
}
</script>

<style>
  
  .footer {
    font-family: 'Footlight MT';
    font-weight: 700;
    background-color: #3d77f6;
    color: black;
    font-size: 18px;
    height: 150px;
    margin: 10px;
    padding: 10px;
  }

  .footer-contact {
    text-align: center;
    margin: 5px;
  }
    
  .footer-copyright {
    font-size: 15px;
    text-align: center;
    margin-top: 65px;
  }

</style>