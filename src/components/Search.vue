<template>
        <div class="searchs" v-if="showSearch">
            <input type="text" class="form-control" placeholder="Search..." aria-label="Search..." aria-describedby="basic-addon1">
        </div>
    <div class="search_box">
        <button class="btn btn-link btn-lg" @click="showSearch =! showSearch" type="button" >
               <!--<i class="bi bi-search"></i>-->
               <svg id="search-outline_copy" data-name="search-outline copy" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <rect id="Rectangle" width="24" height="24" opacity="0"/>
                <path id="Shape" d="M16.29,17.71l-3.39-3.4A7.919,7.919,0,0,1,8,16a8,8,0,1,1,8-8,7.919,7.919,0,0,1-1.69,4.9l3.4,3.39a1,1,0,1,1-1.42,1.42Z" transform="translate(3 3)"/>
                </svg>
        </button>
    </div>
</template>

<style scoped>
.search_box{
    float: right;
}
.searchs {
    width: 80%;
    margin-top: 5px;
    float: left;
}
</style>
<script>
export default {
    data : ()=> ({
    showSearch : false,
  }),
    mounted(){
           
    },
    methods : {

    }

}
</script>