<template>
    <div class="footer">
        <div class="footer_menu">
            <div>
                <ul>
                    <li><a href="#">Newsletter</a></li>
                    <li><a href="#">Contact</a></li>
                    <li><a href="#">Press room</a></li>
                </ul>
            </div>
            <div class="icon_box">
                <i class="bi bi-facebook"></i>
                <i class="bi bi-twitter"></i>
            </div>
        </div>
        <div class="footer_info">
            <div>
                ART GALLERY<br>
                38-40 Southwark Street<br>
                London SE1 1UN<br>
                Telephone +44 20 74905337<br>
            </div>
        </div>
        <div class="footer_copy">
            <div>
                © 2022 EC1 GALLERY
            </div>
        </div>
    </div>
</template>
<style scoped>
.footer{
    width: 100%;
    height: 326px;
    background-color: #424242;
    float: left;
    margin-top: 0px;
    padding: 10px 30px;
}
.footer_menu{
    display: grid;
    grid-template-columns: 75% 25%;
    padding: 10px;
    border-bottom: 1px solid #D8D8D8;
}
.footer_menu div ul {
    margin-left: -55px;
}
.footer_menu div ul li {
    float: left;
}
.footer_menu div ul li a{
    text-decoration: none;
    color: white;
    padding: 10px 15px;
    font-size: 24px;
}
.icon_box i.bi.bi-facebook, i.bi.bi-twitter{
    font-size: 36px;
    color: black;
    margin-left: 25px;
}
.icon_box {
    text-align: right;
}
.footer_info{
    text-align: left;
    color: white;
    font-size: 20px;
    padding: 20px 0;
    border-bottom: 1px solid #D8D8D8;
}
.footer_copy{
    text-align: left;
    color: #ffffff94;
    font-size: 20px;
    padding: 20px 0;
}
</style>