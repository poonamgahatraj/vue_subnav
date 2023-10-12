<template>
    <div class="nav">
        <div>
            <button class="btn1">Home</button>
        <button class="btn" @mouseover="shownav1=true"  @mouseleave="shownav1 = false">About</button>
        
        <button class="btn" @mouseover="shownav2=true"  @mouseleave="shownav2 = false"  >Services</button>
       
        <button class="btn" @mouseover="shownav3=true"  @mouseleave="shownav3 = false">Partner</button>

        <button class="btn1" >Contact</button>

        
        
        
        </div>
       
    </div>
    <div class="btn-content" v-if="shownav1">
            <a >Company</a>
            <a >Team</a>
            <a >Careers</a>
        </div>

        <div class="btn-content" v-if="shownav2">
            <a>Bring</a>
            <a >Deliver</a>
            <a >Package</a>
            <a >Express</a>
        </div>

        <div class="btn-content" v-if="shownav3">
            <a >Link 1</a>
            <a >Link 2</a>
            <a >Link 3</a>
            <a >Link 4</a>
        </div>
</template>

<script>
export default{
    data(){
        return{
            shownav1 : false,
            shownav2 : false,
            shownav3 : false
           
        }
    },
    
}
</script>

<style>
.nav{
    background-color: #333; 
   
    color:white;
    height: 40px;
    
}

.btn{
    background-color: #333; 
    border:none;
    color:white;
    margin-right: 10px;
    font-size: 15px;
    height: 40px;
}

.btn1{
    background-color: #333; 
    border:none;
    color:white;
    margin-right: 10px;
    font-size: 15px;
    height: 40px;
}

.btn1:hover{
    background:red;
    
}

.btn:hover{
    background:red;
    
}

a{
    margin-right: 10px;
}

a:hover{
    background:red;
}
.btn-content{
    padding: 20px;
    background: red;
    
}
</style>