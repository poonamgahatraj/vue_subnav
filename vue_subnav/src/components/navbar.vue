<template>
    <div class="nav">
        <a>Home</a>
        <button class="btn" @click="Showsubnav1">About</button>
        <div class="btn-content" v-if="shownav1">
            <a >Company</a>
            <a >Team</a>
            <a >Careers</a>
        </div>
        <button class="btn" @click="Showsubnav2">Services</button>

        <div class="btn-content" v-if="shownav2">
            <a>Bring</a>
            <a >Deliver</a>
            <a >Package</a>
            <a >Express</a>
        </div>
        <button class="btn" @click="Showsubnav3">Partner</button>

        <div class="btn-content" v-if="shownav3">
            <a >Link 1</a>
            <a >Link 2</a>
            <a >Link 3</a>
            <a >Link 4</a>
        </div>
        <a>Contact</a>
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
    methods:{
        Showsubnav1(){
            this.shownav1=!this.shownav1
        },
        Showsubnav2(){
            this.shownav2=!this.shownav2
        },
        Showsubnav3(){
            this.shownav3=!this.shownav3
        }
    }
}
</script>

<style>
.nav{
    background-color: #333; 
    padding:10px;
    color:white;
    padding:10px;
}

.btn{
    background-color: #333; 
    border:none;
    color:white;
    margin-right: 10px;
}

.btn:hover{
    background:red;
    
}

a{
    margin-right: 10px;
}

.btn-content{
    padding: 10px;
    background: red;
}
</style>