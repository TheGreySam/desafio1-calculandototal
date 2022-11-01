<template>
    <div class="container">
        <div class="row">
         <div class="card col-sm main-bg text-light" style="width: 22rem">
            <img src="@/assets/laptop.jpg" class="card-img-top mx-auto my-5" alt="...">
            <div class="card-body">
                <h5 class="card-title">Laptop Gamer AMD</h5>
                <div class="input mb-3 px-3">
                    <input type="number" class="form-control m-2" id="cantidad" placeholder="Cantidad" aria-label="Cantidad"
                        aria-describedby="button-addon2">
                    <input type="text" class="form-control m-2" id="color" placeholder="Color" aria-label="Color"
                        aria-describedby="button-addon2">
                    <h5>Precio: 400000</h5>
                </div>
                <button class="btn btn-calcular text-light" @click="Calcular">Calcular Total</button>
            </div>
        </div>
        <div class="card col-sm" id="totaltotal" style="width: 22rem">
            
        </div>
       </div>
    </div>
   
</template>
  
<script>
    export default {
  name: 'CalculatorView',
  //data: () => ({
    //cant: "0"
  //}),
  
  methods: {
    //Calcular() {
      //  document.querySelector(".cantidad").parseInt = "0"
      Calcular()  {    
        let cantidad = document.querySelector("#cantidad").value;
        let color = document.querySelector("#color").value;
        document.querySelector("#totaltotal").innerHTML = 
        `<div class="card-body ">
            <h5>Total= $${cantidad * 40000}</h5>
            <h5>Cantidad= ${cantidad}</h5>
            <h5>Color= 
                <span style="height: 25px; width: 25px; border-radius: 50%; background-color: ${color}; display: inline-block">  
                    <span/>
        </h5>
        </div>`;
      }
    }
  }
  //const cant = document.querySelector(".cantidad");
  //computed: {
    
    //CantidadTotal() {
      //return (this.cantidad);
    //}
  //}
 
//}
   


    
 
</script>
  
<style scoped>
.card img {
    object-fit: cover;
    max-width: 20rem;
    height: 14rem;
}

.btn-calcular {
    background-color: orange;
}

.main-bg {
    background-color: rgb(105, 175, 0);
    width: 22rem;
}
</style>
  