<template>
    <div>
        <div class="imagen">
            <img src="../assets/banco.jpg" 
            alt="Girl in a jacket" 
            width="400%" 
            height="300%">
        </div>
        <div class="barraNavegacion">
        <b-navbar class="barra">
        
        <template slot="start">
            <b-navbar-item href="#"> .Creditos.</b-navbar-item>
            <b-navbar-item href="#"> .Leasing.</b-navbar-item>
            <b-navbar-item href="#"> .Ahorros.</b-navbar-item>
            <b-navbar-item href="#"> .Servicio al cliente.</b-navbar-item>
           
        </template>

        <template slot="end">
            <b-navbar-item tag="div">
                
            </b-navbar-item>
        </template>
    </b-navbar>
        </div>
        
       
    </div>    
</template>


<script>
export default {
     data() {
            return {
                rounded: false
            };
        }
};
</script>


<style scoped>
.barra{
    background-color: #ffd400;
}
.imagen{
    background-color: #ffd400;
}

</style>