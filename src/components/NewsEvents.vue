<template>
    <div class="news_events">
        <div class="top_info_box">
            <div class="left">
                <span>
                    News & Events
                </span>
            </div>
            <div class="right">
                <a href="#">
                <span>
                    View all<i class="bi bi-arrow-right-short"></i>
                </span>
                </a>
            </div>
        </div><!--end top info-->
        <div class="news_events_post_box">
            <div class="post_box">
                <a href="#">
                <div class="image_box">
                    <img src="../assets/01.png" alt="art gallery">
                </div>
                <div class="post_text_box">
                    <div class="title">
                        Exhibition: He Xiangyu monograph released by Distanz
                        From March 2016
                    </div>
                    <p class="card-text">
                        He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016
                    </p>
                </div>
                </a>
            </div>
            <div class="post_box">
                <a href="#">
                <div class="image_box">
                    <img src="../assets/02.png" alt="art gallery">
                </div>
                <div class="post_text_box">
                    <div class="title">
                        Exhibition: He Xiangyu monograph released by Distanz
                        From March 2016
                    </div>
                    <p class="card-text">
                        He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016
                    </p>
                </div>
                </a>
            </div>
            <div class="post_box">
                <a href="#">
                <div class="image_box">
                    <img src="../assets/03.png" alt="art gallery">
                </div>
                <div class="post_text_box">
                    <div class="title">
                        Preview: White Cube Mason’s Yard
                        19 January 2017, 6 to 8pm Join us at Mason's Yard
                    </div>
                    <p class="card-text">
                        London for the preview of the new Park Seo-Bo exhibition curated by Katharine Kostyál. Curated by Katharine Kostyál
                    </p>
                </div>
                </a>
            </div>
            
            
            
            <!--
            <div class="post_box" v-for="data in newsData" :key="data.id">
                <div class="image_box">
                    <img :src="data.img" alt="art gallery">
                </div>
                <div class="post_text_box"><p>{{data.description}}</p>
                </div>
            </div>-->

        </div>
    </div>
</template>
<script>
export default {
    data : ()=> ({
        newsData  :[
            {
                id : 1,
                img: 'http://localhost:8080/img/01.png',
                title : 'Exhibition: He Xiangyu monograph released by Distanz From March 2016',
                description : 'He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016',

            },
            {
                id : 2,
                img: '../assets/02.png',
                title : 'Exhibition: He Xiangyu monograph released by Distanz From March 2016',
                description : 'He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016',

            },
            {
                id : 3,
                img: '../assets/03.png',
                title : 'Preview: White Cube Mason’s Yard 19 January 2017, 6 to 8pm<br>Join us at Mason s Yard',
                description : 'London for the preview of the new Park Seo-Bo exhibition curated by Katharine Kostyál. Curated by Katharine Kostyál',

            }
        ]
    }),
    mounted(){
           
    },
    methods : {

    }
}
</script>
<style scoped>
    .news_events{
        width: 100%;
        height: 600px;
       /* background-color: brown;*/
        float: left;
        margin-top: 50px;
        border-top: 1px solid #D8D8D8;
    }
    .top_info_box{
        display: grid;
        grid-template-columns: 50% 50%;
        font-size: 24px;
        padding: 10px 0;
    }
    .top_info_box .left{
        text-align: left;
         font-family: "DINPro-Bold";
    }
    .top_info_box .right{
        text-align: right;
        font-family: "DINPro-Medium";
    }
.top_info_box .right a{
         text-decoration: none;
         color: #222222;
    }
    .top_info_box .right a:hover{
        text-decoration: underline;
    }
    .news_events_post_box{
        display: grid;
        grid-template-columns: 330px 330px 300px;
    }
    .image_box{
        width: 300px;
        height: 300px;
    }
    .image_box img{
        width: 100%;
    }
    .post_text_box {
    width: 94%;
    height: 215px;
    text-align: left;
    margin-top: 15px;
    position: relative;
    overflow: hidden;
}
.post_box {
    position: relative;
    overflow: hidden;
}
   .post_box a{
       text-decoration: none;
       float: left;
           transition: all .3s cubic-bezier(.25,.1,.25,1);
           position: relative;
   }
   .post_box a:hover{
       text-decoration: underline;
       transform: translate(0,-5px);
   }
   .post_box a:hover:after {
    transform: translateX(0);
 
}
.post_box a:after {
    content: "open";
    width: 50px;

    transform: translateX(-70px);
    background: #ffd400;
    position: absolute;
    border-radius: 16px;
    top: 30%;
    left: 6px;    -webkit-transition: -webkit-transform .3s cubic-bezier(.25,.1,.25,1);
    transition: -webkit-transform .3s cubic-bezier(.25,.1,.25,1);
    transition: transform .3s cubic-bezier(.25,.1,.25,1);
    transition: transform .5s cubic-bezier(.25,.1,.25,1),-webkit-transform .5s cubic-bezier(.25,.1,.25,1);
    -webkit-transition-delay: .15s;
    }
   .post_text_box .title{
       font-family: "DINPro-Bold";
       text-decoration: none;
       font-size: 20px;
       color: #222222;
       margin-bottom: 10px;
   }
      .post_text_box P{
          font-size: 20px;
           font-family: "DINPro-Medium";
           color: #222222;
      }
   @media (max-width: 768px) {
       .news_events_post_box{
           display: block;
       }
       .news_events{
           height: 100%;
           margin-top:30px;
       }
       .image_box{
           width: 100%;
           height: 100%;
       }
   }
</style>