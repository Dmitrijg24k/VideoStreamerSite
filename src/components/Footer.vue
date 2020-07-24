<template>
    <div class="footer">
        <div class="copy">
            <div class="container">
                <!-- <div class="row justify-content-end">
                    <div class="col-lg-4">
                        <p class="footerInfo">
                            <span id="city">Астрахань</span><br>
                            Кулаковский промузел, ул. Широкая, д.1 <br>
                            <span class="info">mail: </span><span id="mail">strim@roditelskiy.site</span><br>
                            <span class="info">тел: </span><span id="number">8-961-056-5442</span>
                        </p>
                    </div>
                </div> -->
                <div class="row">
                    <div class="col-lg-8 align-self-end">
                        <span class="copyright">&copy; Айти Глобал Сервис Групп 2020</span>
                    </div>
                     <div class="col-lg-4">
                        <h4>Контакты</h4> 
                        <p class="footerInfo">
                            <span id="city">Астрахань</span><br>
                            Кулаковский промузел, ул. Широкая, д.1 <br>
                            <span class="info">mail: </span><span id="mail">strim@roditelskiy.site</span><br>
                            <span class="info">тел: </span><span id="number">8-961-056-5442</span>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    .footer{
        background-color: #003b32;
        h4{
            margin: 10px 0 20px;
            text-align: right;
            font-weight: 100;
            font-size: 20px;
            color: #A60911;
        }
        .footerInfo{
            padding-bottom: 20px;
            text-align: right;
            font-size: 16px;
            font-weight: 200;
            color: #cbcaaf;
            #city{
                font-size: 18px;
                color: #ff1b24;
                margin: 15px 0 25px;
            }
            #mail, #number{
                color: #0083bf;
            }
        }
        .copyright{
            display: block;
            //width: 100px;
            text-align: left;
            padding: 5px 0px 20px;
            font-size: 14px;
            color: rgb(201, 196, 196);
        }
    }
</style>