<template>
    <el-main class="course-page">
        <router-link to="/courses">
        <el-page-header class="block" title="Вернуться">
        </el-page-header>
        </router-link>
        <div class="title block">
            <h1>Название курса</h1>
        </div>
        <div class="info block">
            <div class="hashtags">
                <el-row :gutter="20">
                    <el-col :span="4"># 1-3 года</el-col>
                    <el-col :span="4"># 3-5 лет</el-col>
                    <el-col :span="4"># Подготовка</el-col>
                </el-row>
            </div>
            <div class="duration">
                <p>30 дней</p>
                <p>14 заданий</p>
                <p>60 уроков</p>
                <p>Чат</p>
            </div>
        </div>
        <div class="about block">
            <div class="info">
                <p>О чем этот курс</p>
                <p><bold>Практики, техники и четкие шаги, как наладить процесс воспитания от А до Я.</bold> У нас тоже не сразу появились 7 детей и понимание, что родительство может быть Счастливым, без жертв и конфликтов.</p>
            </div>
            <div class="leftbox video">
                    <video src=""></video>
            </div>
            <div class="rightbox">
                <div class="">
                    <p>Когда был 1 ребёнок, то ошибок было в сотни раз больше, чем сейчас. Да, сейчас они тоже есть, но уже другого порядка. А базовая система воспитания ясна и раскладывается на ступени лестницы, по которой я вас проведу.</p>
                    <button>Показать больше</button>
                </div>
                <button>Купить за 1 199 р.</button>
            </div>
        </div>
        <div class="course-program block">
            <h3>Программа курса</h3>
            <div class="program-list">
                <router-link to="/courses/course-page/video-lesson"><div class="program-list-item">1. Основы основ ухода</div></router-link>
                <div class="program-list-item">2. Правильная гигиена</div>
                <div class="program-list-item">3. Как правильно разговаривать с ребенком</div>
                <div class="program-list-item">4. Чем кормить ребенка 3-5 лет</div>
                <div class="program-list-item">1. Основы основ ухода</div>
                <div class="program-list-item">1. Основы основ ухода</div>
                <div class="program-list-item">1. Основы основ ухода</div>
                <div class="program-list-item">1. Основы основ ухода</div>
            </div>
            <button>Показать всю программу</button>
        </div>
        <div class="reasons-to-take block">
            <div class="leftbox">
                <h2>Этот курс для Вас, если</h2>
                <ul>
                    <li>иметь красивое здоровое тело</li>
                    <li>быть в тонусе, а не валиться от усталости</li>
                    <li>успевать жить ярко, проживая СВОЮ жизнь</li>
                    <li>вдохновлять близких своим примером</li>
                </ul>
            </div>
            <div class="rightbox">
                <h3>Негативные последствия, если ничего не менять</h3>
                <ol>
                    <li>Ребенок видит модель вашего дурного примера</li>
                    <li>Нет благодарности в ответ на ваши старания</li>
                    <li>Вы пролетаете мимо самого важного</li>
                    <li>Нет близости с детьми, нет доверия</li>
                    <li>Вечные усталость и недосып</li>
                    <li>Вы живете в страхе за будущее детей</li>
                    <li>Дети растут в атмосфере крика и раздражения</li>
                </ol>
            </div>
            <div class="faq">
                <h2>Как проходит курс</h2>
                <div class="faq-item">
                    <img src="">
                    <div class="item-question">
                        <h4>Что же внутри?</h4>
                        <p>Каждые 2-3 дня на платформе появляется новый урок. Вам приходит уведомление. Вы можете двигаться в своем темпе, но оптимальнее - с потоком, так как участницы часто зеркалят друг друга, помогают, заряжают и мотивируют.</p>
                    </div>
                </div>
                <div class="faq-item">
                    <img src="">
                    <div class="item-question">
                        <h4>А я успею все посмотреть?</h4>
                        <p>Все видеоуроки - по 15-20 минут. Вы смотрите их в любое удобное время через телефон, планшет или компьютер. Вы можете впитывать знания на прогулке с ребенком или где угодно. Все записи доступны до окончания курса.</p>
                    </div>
                </div>
                <div class="faq-item">
                    <img src="">
                    <div class="item-question">
                        <h4>Какой прогресс Вас ждет?</h4>
                        <p>Мы делаем замеры ключевых показателей ДО курса и ПОСЛЕ, результаты будут очевидны и приятны. После урока есть практические задания, вы встраиваете их в свою жизнь, и после - можете делиться успехами в отчете. Это эффективно.</p>
                    </div>
                </div>
            </div>
            <div class="gray">
                <h2>В результате Вы узнаете</h2>
                <p>Как исправить недочеты в прошлом, серьезно проинвестировать в будущее семьи и ребёнка</p>
                <div class="points-list">
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                    <div class="points-list-item">
                        <img src="">
                        <div class="content">
                            <h5>Детские истерики</h5>
                            <p>Как реагировать на детские недовольство/кризисы возрастов</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="reviews">
                <div class="title">
                    <h2>Отзывы</h2>
                    <p>17 отзывов</p>
                </div>
            </div>
            <div class="gray reasons">
                <h2>Почему вы можете мне доверять?</h2>
                <div class="reasons-list">
                    <div class="reason">
                        <h4>30 лет супружества</h4>
                        <p>Романтика и влюбленность даже спустя 30 лет? Легко! Я знаю секреты счастья.</p>
                    </div>
                    <div class="reason">
                        <h4>500+ принятых родов</h4>
                        <p>Веду беременность, помогаю в родах, 5 000 часов патронажа детей + семейных пар.</p>
                    </div>
                    <div class="reason">
                        <h4>120 лет материнства</h4>
                        <p>У меня 7 детей и 2 внучки. Вижу подрастающие плоды нашего воспитания.</p>
                    </div>
                    <div class="reason">
                        <h4>3 образования</h4>
                        <p>Включая медицинское + постоянные курсы повышения квалификации, саморазвитие.</p>
                    </div>
                </div>
            </div>
            <div class="to-buy">
                <div class="gray">
                    <bold>В университетах не учат воспитывать детей.</bold> Вы сразу тренируетесь на своих детях. И цена ошибки очень высока. Но если рядом есть семья с положительным примером воспитания, то вам остается только перенять опыт, внедрить и пользоваться на благо.
                </div>
                <button>Купить за 1 199 р.</button>
            </div>
        </div>
        <div class="infobox  block">
            <div class="comments">
                <div class="title">
                    <h3>Комментарии</h3>
                    <p>3</p>
                </div>
                <input placeholder="Написать комментарий">
                <div class="filters">
                    <button>Популярные</button>
                    <button>Новые</button>
                </div>
                <el-divider></el-divider>
                
            </div>
        </div>
    </el-main>
</template>
<script>
export default {
    name: "CoursePage"
}
</script>