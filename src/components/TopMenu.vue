<template>
    <div class="top-menu">
        <div class="container-fluid">
            <nav class="navbar navbar-expand">
                <a href="#" class="logo">Contora</a>
                <div class="menu-items collapse navbar-collapse" id="navbarText">
                    <ul class="navbar-nav">
                        <li class="navbar-item active">
                            <a href="#" class="nav-link">Основные особенности</a>
                        </li>
                        <li class="navbar-item">
                            <a href="#accordion" class="nav-link">Технические возможности</a>
                        </li>
                        <li class="navbar-item active">
                            <a href="#subscribe" class="nav-link">Связаться с нами</a>
                        </li>
                    </ul>
                </div>
                <!-- <div class="actions">
                    <ul class="navbar-nav mr-auto">
                        <li class="nav-item"><a href="#" class="">1</a></li>
                        <li class="nav-item"><a href="#" class="">2</a></li>
                        <li class="nav-item"><a href="#" class="">3</a></li>
                    </ul>
                </div> -->
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>
<style lang="css">
    #accordion{
        border-top: 60px solid transparent;
        margin-top: -60px;
        background-clip: padding-box;
    }
</style>
<style lang="scss" scoped>
    .top-menu{
        position: fixed;
        z-index: 10;
        top: 0;
        left: 0;
        width: 100%;
        padding: 7px 22px;
        transform: box-shadow .3s ease;
        color: #fff;
        height: 70;
        font-weight: 400;
        display: flex;
        background-color: #0f38ab;
        box-shadow: 0 0 20px #000;
    }
    a{
        text-decoration: none;
        color: #fff;
        margin-right: 15px;
    }
    a:hover{
        text-decoration: none;
        color: #fff;
    }
    .logo{
        font-style: italic;
        font-weight: 200;
        display: block;
        width: 200px;
        text-align: left;
        font-size: 21px;
        float: left;
    }
    .menu-items{
        font-style: normal;
        font-weight: 400;
        display: block;
        text-align: left;
        font-size: 18px;
        float: left;
        a{
            display: inline-block;
            padding: 2px 15px;
            border: 1.5px solid #0f38ab;
            transition: 0.5s ease;
        }
        a:hover{
            padding: 2px 15px;
            color: darken(#fff, 10%);
            border: 1.5px solid lighten(#0f38ab, 20%);
        }
    }
   
    .actions{
        font-style: normal;
        font-weight: 600;
        display: block;
        width: 50px;
        text-align: right;
        font-size: 16px;
        float: right;
        margin-right: 50px;
        li{
          margin-right: 15px;  
          a{
            display: inline-block;
            border: 1.5px solid #0f38ab;
            transition: 0.5s ease;
            margin-right: 0px;  
          }
          a:hover{
            color: darken(#fff, 20%);
          }
        }
    }
</style>