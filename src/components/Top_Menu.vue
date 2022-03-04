<template>
    <div>
     
            <button class="btn btn-link btn-lg" type="button" data-bs-toggle="collapse" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
                <!--<i class="bi bi-list"></i>-->
                <svg id="menu-outline" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <rect id="Rectangle" width="24" height="24" transform="translate(24 24) rotate(180)" opacity="0"/>
                <rect id="Rectangle-2" data-name="Rectangle" width="18" height="2" rx="0.95" transform="translate(3 11)"/>
                <rect id="Rectangle-3" data-name="Rectangle" width="18" height="2" rx="0.95" transform="translate(3 16)"/>
                <rect id="Rectangle-4" data-name="Rectangle" width="18" height="2" rx="0.95" transform="translate(3 6)"/>
                </svg>
            </button>
    
        <div class="collapse" id="collapseExample">
        <div class="card card-body" >
                <router-link to="/">Home</router-link> 
                <router-link to="sad">Art & Artists</router-link>
                <router-link to="sda">Exhibitions</router-link> 
                <router-link to="sad">News</router-link>
                <router-link to="about">About</router-link> 
                <router-link to="asd">Private area</router-link>
                <div class="closebtn" @click="closefun">
                    <svg id="close" xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 16 16">
                    <path id="Path" d="M1.825.313A1.069,1.069,0,0,0,.313,1.825L6.488,8,.313,14.175a1.069,1.069,0,1,0,1.512,1.512L8,9.512l6.175,6.175a1.069,1.069,0,0,0,1.512-1.512L9.512,8l6.175-6.175A1.069,1.069,0,0,0,14.175.313L8,6.488Z" transform="translate(0 0)"/>
                    </svg>
                </div>
        </div>
        </div>
    </div>
</template>
<script>
export default {
    data : ()=> ({
    collapse : null,
  }),
    mounted(){
         
    },
    methods : {
        closefun(){
          this.collapse = document.querySelector('.collapse')
          this.collapse.classList.remove('show')
        }

    }

}
</script>
<style scoped>
.closebtn{
    position: absolute;
    top: 50px;
    right: 30px;
    font-size: 28px;
    z-index: 55;
    padding:0 11px;
    border-radius: 13px;
}
.closebtn:hover{
    border:1px solide silver;
    background-color: rgb(220 243 144);
    color: white;
    box-shadow: 4px 4px 1px #fbe6e642;
    cursor: pointer;
}
 svg#search-outline_copy:hover{
    background-color:white ;
}   
i.bi.bi-list {
    color: black;
    font-weight: bold;
    font-size: 28px;
    
}
@media (max-width: 768px) {
    #nav a{
        font-size: 30px;
        line-height: 60px;
    }
    .closebtn{
        top: 27px;
        right: 21px;
    }
}


</style>