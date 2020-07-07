<template>
    <div class="content">
        <div class="selection">
            <div class="container">
                <div class="top-content">
                   <div class="row">
                        <div class="col-lg-7">
                            <h1>Видеостример</h1>
                            <p>
                                Видеостример – обеспечение для сбора, хранения и транспорта видеопотока 
                                с камер до конечного пользователя – видеостример. 
                                Видеостример может стать основой как привычной системы видеонаблюдения, 
                                так и частью более сложных систем (продукт имеет специальное API, 
                                позволяющее организовать взаимодействие с другими программными продуктами: 
                                например, передачу видеопотока пользовательскому приложению). 
                                Данный продукт позволяет организовать живую видеотрансляцию с 
                                предоставлением массового доступа к видео, запись и хранение видеопотока 
                                на сервере, а также предоставление архивного видео пользователям по запросу. 
                            </p>
                        </div>
                        <div class="col-lg-5">
                            <img src="./../assets/camDarkBlue.png" alt="">
                        </div>
                   </div>
                </div>
                <div class="gears">
                    <div class="row">
                        <div class="col-lg-4">
                            <img src="./../assets/twogears.svg" alt="">
                        </div>
                        <div class="col-lg-8">
                            <h3>Надёжная защита</h3>
                            <p>
                                Для защиты данных от распространения видеоконтента 
                                неавторизованным пользователям в системе предусмотрен 
                                механизм проверки токена авторизаци.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="middle">
                    <div class="row justify-content-between">
                        <div class="col-lg-7">
                            <h3>Широкие возможности</h3>
                            <p>
                                Глубина архива настраивается для каждой камеры отдельно. 
                                Также, при необходимости, можно настроить время суток, когда необходимо писать архив.
                            </p>
                            <p>
                                Место хранения для каждой камеры настраивается индивидуально. 
                                При необходимости, камеру можно отключить, не удаляя ее из общего списка камер.
                            </p>
                        </div>
                        <div class="col-lg-4">
                            <img src="./../assets/camLeft.png" alt="">
                        </div>
                    </div>
                </div>
                <div class="penultimate-content">
                    <div class="row">
                        <div class="col-lg-4">
                            <img src="./../assets/diagramBlue.svg" alt="">
                        </div>
                        <div class="col-lg-8">
                            <h3>Оценка производительности</h3>
                            <p>
                                Операционная система: Ubuntu 18.04 версии и выше;
                                Железо: Процессор (CPU Xeon E5620 2.40 GHz) 2 шт., Оперативная память 32Gb RAM;
                                Расчетная производительность: 1200-1300 камер.
                            </p>
                            <p>
                                При более производительном оборудовании конечное количество камер упирается 
                                в ограничение пропускной способности сетевого канала и ограничение объема архивного хранилища.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="bottom-content">
                    <div class="row">
                        <div class="col-lg-8">
                            <h3>Условия тестового использования</h3>
                            <p>
                                Мы предлагаем ознакомится с нашим программным продуктом на следующих условиях: 
                            </p>
                            <p>
                                -	Бесплатный тестовый период - 60 дней. <br>
                                -	Полный функционал программы. <br>
                                -	Полная техническая поддержка и исправление выявленных ошибок. <br>  
                                -	Льготные цены после завершения бесплатного тестового периода. <br>
                            </p>
                        </div>
                        <div class="col-lg-4">
                            <img src="./../assets/testdrive.svg" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="accordion" id = "accordion">
            <div @click="dropInfoStatus = !dropInfoStatus" 
                class="drop-block">
                 <div class="container">
                    <h2 id="accordion"><font-awesome-icon icon="chevron-circle-down" /><span>Технические характеристики и возможности</span></h2>
                 </div>
            </div>
            <transition name="drop-info-transition">
                <div v-if="dropInfoStatus" class="drop-info" v-transition>
                    <div class="container">
                        <div class="row justify-content-around">
                            <div class="col-lg-5">
                                <h4>Поддерживаемый функционал</h4>
                                <ul>
                                    <li>
                                        Получение RTSP видеопотока и его сохранение в .ts 
                                        файлы для последующей компоновки в HLS поток (m3u8 медиа-листы).
                                    </li>
                                    <li>
                                        Видео-трансляции с IP-камер в режиме реального времени.
                                    </li>
                                    <li>
                                        Вывод медиа-листа для запрашиваемого промежутка времени (архив).
                                    </li>
                                    <li>
                                        Проверка токена безопасности для работы с программой.
                                    </li>
                                    <li>
                                        Экспорт архивного видеопотока в mp4 файл.
                                    </li>
                                    <li>
                                        Сохранение видеопотока камеры с аудиопотоком другой имеющейся камеры.
                                    </li>
                                    <li>
                                        Автоматическая очистка архива по срабатыванию (глубина архива).
                                    </li>
                                    <li>
                                        Возможность управления и мониторинга стримера по API.
                                    </li>                          
                                </ul>
                            </div>
                            <div class="col-lg-5">
                                <h4>Веб-интерфейс</h4>
                                <p>В панели администратора можно увидеть такую информацию как:</p>
                                <ul>
                                    <li>Текущее время работы системы; 
                                    </li>
                                    <li>Текущий сетевой поток;
                                    </li>
                                    <li>Текущее использование CPU;
                                    </li>
                                    <li>Общее количество камер/ количество подключенных;
                                    </li>
                                    <li>Битрейт для каждой подключенной камеры;
                                    </li>
                                    <li>Состояние каждой камеры;
                                    </li>
                                    <li>Количество подключений к камере со стороны стримера за время работы.
                                    </li>

                                </ul> 
                            </div>
                        </div>
                        <div class="row justify-content-around">
                            <div class="col-lg-5">
                                <h4>Принцип работы</h4>
                                <p>Работа стримера идёт по принципу:</p>
                                <ul>
                                    <li>
                                        Захват с IP-камеры по rtsp протоколу
                                    </li>
                                    <li>
                                        Кодирование и запись в архивном хранилище
                                    </li>
                                    <li>
                                        Доставка до конечного пользователя по hls протоколу
                                    </li>
                                </ul>
                            </div>
                            <div class="col-lg-5">
                                <h4>Веб-интерфейс</h4>
                                <p>Также в панели администратора можно производить такие действия как:</p>
                                <ul>
                                    <li>
                                        Добавление новых камер; 
                                    </li>
                                    <li>
                                        Просмотр истории (архив онлайн) для конкретной камеры;
                                    </li>
                                    <li>
                                        Получение архива за заданный промежуток времени в формате mp4 файла для конкретной камеры;
                                    </li>
                                    <li>
                                        Просмотр конкретной камеры онлайн.
                                    </li>
                                </ul> 
                            </div>
                        </div>
                        <div class="row justify-content-around">
                            <div class="col-lg-5">
                                <h4>Производительность</h4>
                                <p>Сервер:</p>
                                <ul>
                                    <li>
                                        Операционная система: Ubuntu 16.04 версии и выше;
                                    </li>
                                    <li>
                                        Железо: Процессор (CPU Xeon E5620 2.40 GHz) 2 шт., Оперативная память 32Gb RAM;
                                    </li>
                                    <li>
                                        Расчетная производительность: 1200-1300 камер.
                                    </li>
                                </ul>
                            </div>
                            <div class="col-lg-5">
                                <h4>Веб-интерфейс</h4>
                                <p>Другие возможности веб-интерфейса:</p>
                                <ul>
                                    <li>
                                        Доступ  и конфигурация сервера через браузер
                                    </li>
                                    <li>
                                        Не используется ActiveX плагинов
                                    </li>
                                    <li>
                                        Доступ к статистике и мониторингу
                                    </li>
                                </ul> 
                            </div>
                        </div>
                    </div>
                </div>
            </transition>
        </div>
        <div class="conection">
            <div class="container">
                <div class="row">
                    <div class="col-lg-6">
                        <h2>Получить пробную версию </h2>
                        <form action="#" method="get">
                            <div class="form-item">
                                <input type="text" name="name" id="name" placeholder="Ваше имя">
                            </div>  
                            <div class="form-item">
                                <input type="email" name="email" id="" placeholder="Ваш email">
                            </div>  
                            <div class="form-item">
                                <label for="textarea">Опишите вашу компанию</label>
                                <textarea name="description" id="description" cols="30" rows="10"></textarea>
                            </div>  
                            <div class="form-item-button">
                               <input type="button" value="Отправить заявку">
                            </div> 
                        </form>
                    </div>
                    <div class="col-lg-6">
                        <div class="form-info" id = "form-info">
                            <h4>О компании</h4>
                            <p>Разработка программного обеспечения – основное направление деятельности компании Айти Глобал Сервис Групп. <br> В своей работе наша компания использует самые современные методологии разработки программного обеспечения.</p>
                        </div>
                    </div>
                </div> 
            </div>
        </div>
        <button class="open-button" v-on:click="openForm">Обратная связь</button>
        <div class="chat-popup" id="myForm">
        <form action="../action_page.php" class="form-container">
            <h2>Обратная связь</h2>

            <label for="msg"><b>Введите ваш email</b></label>
            <input class="chat-mail" type="email" name="email" id="" placeholder="email">
            <textarea placeholder="Сообщение.." name="msg" required></textarea>

            <button type="submit" class="btn">Отправить</button>
            <span class="close" v-on:click="closeForm"></span>
        </form>
        </div>
    </div>    
</template>
<script>
export default {
    name: 'Content',
    data(){
        return{
            dropInfoStatus: false
        }
    },
    methods: {
        openForm : function () {
            document.getElementById("myForm").style.display = "block";
        },
        closeForm : function () {
            document.getElementById("myForm").style.display = "none";
        }
    }
}
</script>

<style lang="scss" scoped>
    .content{
        padding-top: 71px;
        background-color: #31a881;
        color: #fff;
        text-align: left;
        .top-content{
            margin-bottom: 15px;
            h1{
                margin-top: 80px;
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 48px;
            }
            p{
                font-style: normal;
                font-weight: 400;
                display: block;
                font-size: 17px;
            }
            button{
                transition: 1s linear;
                padding: 8px 16px;
                background-color: #e83333;
                border: 2px solid #e83333;
                color: #fff;
                font-size: 19px;  
                font-weight: 500;
                border-radius: 4px;
            }
            button:hover{
                background-color:  #e78f2a;
                border: 2px solid #e78f2a;
                border-radius: 6px;
            }
            img{
                margin-top: -16px;
                margin-left: -40px;
                width: 500px;
            }
        }
        .gears{
            margin-top: 0px;
            margin-bottom: 15px;
            h3{
                margin-top: 70px;
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 28px;
            }
            p{
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 17px;
            }
        }
        .middle{
            margin-bottom: 15px;
            h3{
                margin-top: 30px;
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 28px;
            }
            p{
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 17px;
                span{
                    display: block;
                    width: 78%;
                    padding-bottom: 1px;
                    //border-bottom: 1.4px solid rgba(255, 255, 255, 0.685);
                }
            }
            img{
                margin-top: 20px;
            }
        }
        .penultimate-content{
            h3{
                margin-top: 60px;
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 28px;
            }
            p{
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 17px;
            }
            img{
                margin-top: 0px;
            }
        }
        .bottom-content{
            padding-bottom: 35px;
            h3{
                margin-top: 60px;
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 28px;
            }
            p{
                font-style: normal;
                font-weight: 100;
                display: block;
                font-size: 17px;
            }
            img{
                margin-top: 35px;
            }
        }
    }
    .accordion{
        display: block;
        width: 100%;
        color: #fff;
        background-color: #3c8890;
        //background-color: #42A7A7;
        .drop-block{
            background-color: #00836f;
            transition: .3s ease;
            padding: 15px 15px 5px 15px;
            h2{
                font-size: 40px;
                margin-left: 0px;
                span{
                    margin-left: 20px;
                }
            }
        }
        /*.drop-block:hover{
            background-color: #a3d0b5;
            color: #fff;
            cursor: pointer;
        }*/
        .drop-info{
            background-color: #31a881;
            padding-top: 60px;
            transition: all .3s ease;
            h4{
                margin-bottom: 15px;
                font-style: normal;
                font-weight: 200;
                display: block;
                font-size: 38px;
                color: #f2f3f4;
                transition: all .6s ease;
            }
            p{
                font-size:  19px;
            }
            h4:hover{
                color: #faebd7;
                cursor: pointer;
            }
            ul{
                padding-left: 20px; 
                list-style-type: none;
                margin-bottom: 20px;
                li{
                    position: relative;
                    margin: 5px 0px 10px 15px;
                }
                li:before{
                    position: absolute;
                    content: "";
                    top: 10px;
                    left: -15px;
                    border-radius: 50%;
                    background-color: rgb(214, 206, 206);
                    width: 4px;
                    height: 4px;
                }
            }
        }
        .drop-info-transition-enter-active, .fade-leave-active {
            transition: all 0.8s ease;
            height: 600px;
            background-color: #31a881;
            overflow: hidden;
        }
        .drop-info-transition-enter, .drop-info-transition-leave-to /* .fade-leave-active до версии 2.1.8 */ {
            height: 0;
            padding: 0 10px;
            opacity: 0;
        }
    }
    .conection{
        padding-top: 80px;
        padding-bottom: 40px;
        border-bottom: 1px solid rgba(153, 153, 153, 0.658);
        background-color: #e0e8e5;
        color: #000000e5;
        .form-info{
            margin-top: 100px;
        }
        a{
            font-size: 16px;
            color: #000000;
            transition: all .2 ease;
            h4{
                color: #5a9696;
                font-size: 18px;
            }
        }
        p{
            font-size: 16px;
        }
        h2{
            color: #111111af;
            font-size: 42px;
            font-weight: 500;
            font-family: EBGaramond, Helvetica, Arial, sans-serif;
        }
        form{
            .form-item{
                input{
                    display: block; 
                    height: 40px;
                    width: 100%;
                    border: none;
                    border-bottom: 1.3px solid #11111133;
                    border-radius: 2px;
                    margin: 15px 0px;
                    color: #11111162;
                    font-size: 24px;
                    font-weight: 500;
                }
                textarea{
                    overflow: auto;
                    resize: none;
                    overflow-wrap: break-word;
                    min-height: 55px;
                    display: block; 
                    height: 55px;
                    width: 100%;
                    border: 1.3px solid #11111133;
                    border-radius: 4px;
                    margin-bottom: 15px;
                }
                label{
                    display: block;
                    width: 100%;
                    margin: 5px 0px;
                    color: #11111162;
                    font-size: 24px;
                    font-weight: 500;
                }
                p{
                    display: block;
                    width: 100%;
                    margin: 5px 0px 15px;
                    color: #111111e5;
                    font-size: 15px;
                    font-weight: 400;
                    a{
                        color: #42A7A7;
                        font-size: 15px;
                        font-weight: 400;
                    }
                }
            }
            .form-item-checkbox{
                input{
                    display: inline-block; 
                    height: 16px;
                    width: 16px;
                    border-radius: 2px;
                    margin: 10px 0px;
                    color: #11111162;
                    font-size: 24px;
                    font-weight: 500;
                }
                label{
                    display: inline-block;
                    width: 80%;
                    margin-left: 15px;
                    color: #11111162;
                    font-size: 16px;
                    font-weight: 800;
                    text-transform: uppercase;
                    font-weight: 500;
                }
            }
            .form-item-button{
                input{
                    display: block;
                    width: 100%;
                    margin: 5px 0px 15px;
                    padding: 15px 20px;
                    background-color: #42A7A7;
                    text-align: center;
                    color: #eeeeeee5;
                    border: 1px solid #42A7A7;
                    text-transform: uppercase;
                    font-size: 15px;
                    font-weight: 500;
                    transition: all .9s ease-in-out;
                }
                input:hover{
                    background-color: #5d8d5d;
                    border: 1px solid #5d8d5d;
                }
            }
        }
    }
    .open-button {
        background-color: #555;
        color: white;
        padding: 8px 10px 25px 10px;
        border: none;
        cursor: pointer;
        opacity: 0.8;
        position: fixed;
        bottom: -25px;
        right: 28px;
        width: 240px;
        border: none;
        border-radius: 30px;
    }
    /* Всплывающий чат - скрыт по умолчанию */
    .chat-popup {
        display: none;
        position: fixed;
        bottom: 0;
        right: 15px;
        border: 3px solid #f1f1f1;
        border-radius: 5px;
        z-index: 9;
        color:#101010d8;
        animation: go-top 2s 1 alternate;
        -webkit-animation: go-top 2s 1 alternate;
    }

    /* Добавить стили для контейнера формы */
    .form-container {
        max-width: 300px;
        padding: 10px;
        background-color: white;
    }
    @keyframes go-top {   
        from {
            bottom: -516px;      
        }
        to {
            bottom: 0px; 
        }
    }

    /* Префикс для Chrome, Opera, Safari */
    @-webkit-keyframes go-top {
        from {
            bottom: -516px;
        }
        to {
            bottom: 0px;
        }
    }
    .chat-mail {
        width: 100%;
        padding: 5px;
        margin: 5px 0px 5px 0px;
        border: 1px solid #f1f1f1;
        border-radius: 5px;
        background: #f1f1f1;
        resize: none;
        min-height: 20px;
    }
    /* Полная ширина текстовой области */
    .form-container textarea {
        width: 100%;
        padding: 5px;
        margin: 5px 0 22px 0;
        border: 1px solid #f1f1f1;
        border-radius: 5px;
        background: #f1f1f1;
        resize: none;
        min-height: 200px;
    }

    /* Когда текстовое поле получает фокус, сделайте что-нибудь */
    .form-container textarea:focus {
        background-color: #ddd;
        outline: none;
    }

    /* Установите стиль для кнопки отправить/войти */
    .form-container .btn {
        background-color: #4CAF50;
        color: white;
        padding: 16px 20px;
        border: none;
        cursor: pointer;
        width: 100%;
        margin-bottom:10px;
        opacity: 0.8;
    }

    /* Добавить красный цвет фона для кнопки "Отмена" */
    .form-container .cancel {
        background-color: red;
    }

    /* Добавить некоторые эффекты наведения на кнопки */
    .form-container .btn:hover, .open-button:hover {
        opacity: 1;
    }
    .close {
        position: absolute;
        right: 4px;
        top: 4px;
        width: 16px;
        height: 16px;
        opacity: 0.3;
        cursor: pointer;
    }
    .close:hover {
        opacity: 1;
    }
    .close:before, .close:after {
        position: absolute;
        left: 2px;
        content: ' ';
        height: 25px;
        width: 3px;
        background-color: #333;
    }
    .close:before {
        transform: rotate(45deg);
    }
    .close:after {
        transform: rotate(-45deg);
    }
</style>