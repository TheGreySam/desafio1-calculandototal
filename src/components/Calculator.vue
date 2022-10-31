<template>
    <div class="hello">
        <div class="card main-bg text-light">
            <img src="@/assets/laptop.jpg" class="card-img-top mx-auto my-5" alt="...">
            <div class="card-body">
                <h5 class="card-title">Laptop Gamer AMD</h5>
                <div class="input mb-3 px-3">
  <input type="text" class="form-control m-2" placeholder="Cantidad" aria-label="Cantidad" aria-describedby="button-addon2">
  <input type="text" class="form-control m-2" placeholder="Color" aria-label="Cantidad" aria-describedby="button-addon2">
  <h5>Precio: 400000</h5>
 
</div>
                <button class="btn btn-calcular text-light">Calcular Total</button>
                
            </div>
        </div>
        <div class="card">
            
            <div class="card-body" style="width: 22rem">
                <h5>Total= $</h5>
                <h5>Cantidad=</h5>
                <h5>Color= </h5>
            </div>
        </div>


    </div>
</template>
  
<script>
export default {
    name: 'HelloWorld',
    props: {
        msg: String
    }
}
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
  