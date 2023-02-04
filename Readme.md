<div class="up-project__info"><h3>Основной проект</h3><p>«Таинственный отпуск» — ваш основной проект. Это ваш главный проект на этом курсе. Выполняя домашние задания и консультируясь со своим наставником, вы будете работать над этим проектом, готовя его к защите.</p></div>

  <div class="up-project__info"><h3>Фыйлы проекта</h3>
    <p>Проект уже свёрстан. В течение курса вы сфокусируетесь на главном: супер анимациях.</p>
    <p>Скачать <a href="files/Проект.zip">стартовый шаблон</a>. </p>
  </div>
  
  <div class="up-project__info"><h3 class="up-project__caption">Техническое задание</h3><div class="up-project__specification text-container text-container--module text-container--specification" id="specification"><p><strong>Цель:</strong> Обеспечить пользователям непрерывность восприятия содержания при переходах между разделами сайта и состояниями игры, создать весёлую атмосферу развлечения.</p><p><strong>Задача:</strong> Дополнить сайт конкурса «Таинственный отпуск» UI и UX анимацией, соответствующей дизайну.</p><p>
</p><h2 id="opisanie-proekta">Описание проекта</h2><h3 id="o-proekte">О проекте</h3><p>«Таинственный отпуск» — сайт конкурса-игры, в котором главный приз — путешествие на 14 дней.</p><p>В процессе конкурса игрокам предстоит угадать пункт назначения путешествия. Победитель может воспользоваться путевкой сам, либо подарить её другу. Время путешествия победитель выбирает самостоятельно в пределах двух лет.</p><h3 id="opisanie-funktsionalnosti">Описание функциональности</h3><p>Сайт представляет собой одностраничный лендинг. Лендинг состоит из разделов высотой в один экран. Прокрутка страницы происходит полной сменой одного экрана. Пока происходит переход между экранами и анимациями, прокрутка заблокирована.</p><p>Список разделов:</p><ol><li>Начало.</li><li>История:

    <ul><li>— Глава 1;</li><li>— Глава 2;</li><li>— Глава 3;</li><li>— Глава 4.</li></ul></li><li>Призы.</li><li>Правила.</li><li>Игра.</li></ol><p>На последнем экране размещается «Игра».</p><h4 id="mekhanika-konkursa-igri">Механика конкурса-игры</h4><p>Для того, чтобы угадать пункт назначения путешествия игрокам необходимо сыграть с ботом <strong>ИИ «Соня»</strong> в Да-Нет-ки: задавать закрытые вопросы, на которые можно ответить только «Да» или «Нет».</p><ol><li>Игрок нажимает «Погнали».</li><li>Запускается таймер, показывается поле ввода вопроса «Задать вопрос» и кнопка «Узнать».</li><li>Пользователь задает вопросы вводя в поле и нажимая кнопку или <code>Enter</code>.
<ul><li>— В чате выше поля ввода появляется его сообщение.</li></ul></li><li>Бот отвечает только «да» или «нет».
<ul><li>— В чате выше поля ввода появляется поле со спиннером (три точки с зацикленной анимацией), показывающим ожидание ответа. Затем на месте спиннера появляется ответ «Да» или «Нет».</li></ul></li><li>Если пользователь пишет название загаданной локации: Страна/континент + название места: населенного пункта, название горы, озера, нац.парка и т. п., бот отвечает «да» и происходит переход к результатам игры «Победа!».</li><li>Призы раздаются согласно порядку отгадывания:
<ul><li>— 1-3 — путёвка;</li><li>— 4-10 угадал — чемодан от организатора конкурса;</li><li>— 10-910 — промокод на скидку 15%.</li></ul></li><li>Если время вышло, а пользователь не отгадал место назначения, показывается экран результата с сообщением о проигрыше «Не угадал!» и предложением попробовать еще раз — кнопка «Не сдавайся!». Количество попыток не ограничено.</li></ol><p><figure><img src="images/MacBookPro-19.png" alt="Имитация игры в личном проекте" title="Имитация игры в личном проекте"><figcaption>Имитация игры в личном проекте</figcaption></figure></p><p>В личном проекте вместо ответов бота выдаются рандомные ответы «Да» или «Нет». Если в поле вводится вопрос «Это Антарктида?», показывается экран «Победа!» с иллюстрацией моржа, а при вопросе «Антарктида?», показывается экран «Победа!» с иллюстрацией чемодана.</p><h4 id="opisanie-obshchikh-blokov">Описание общих блоков</h4><h5 id="shapka">Шапка</h5><p>Шапка закреплена относительно вьюпорта и всегда присутствует на экране.</p><p><strong>Состав шапки:</strong></p><ul><li>— Логотип компании «Fjord Inc.»;</li><li>— Меню;</li><li>— Ссылки на социальные сети, скрытые за одно кнопкой шеринга.</li></ul><p>Шапка имеет <strong>«цветовую схему»</strong> (3 цвета, в которые окрашены элементы и их состояния):</p><ul><li>— Главный цвет: белый, он не меняется;</li><li>— Второстепенный цвет: цвет иконки шеринга, совпадает с цветом фона;</li><li>— Цвет по наведению: светло-фиолетовый.</li></ul><p>Все состояния приведены на схеме: <code>default</code>, <code>hover</code>, <code>focus</code>, <code>current</code>.</p><p>Аналогичные состояния у других элементов сайта.</p><ul><li><strong>Картинка состояний элементов</strong></li></ul><p>Цветовая схема меняется в сценах Истории:</p><ol><li>Глава 1 — светло-фиолетовая.</li><li>Глава 2 — синяя.</li><li>Глава 3 — голубая.</li><li>Глава 4 — совпадает с цветовой схемой по умолчанию.</li></ol><p>Смена цвета анимируется.</p><h5 id="fon">Фон</h5><p>В разделах «Начало» и «История» присутствует 3D-иллюстрация на фоне. В 3D присутствует 5 сцен, по одной на раздел/главу. При переходе между разделами и главами истории на иллюстрации происходит переход между сценами.</p><p>В оставшихся разделах «Призы», «Правла» и «Игра» 3D-иллюстрация на фоне отсутсвуют. Рендер анимации 3D должен останавливаться, чтобы не загружать ресурсы браузера. Нужно при переходе к этим разделам сделать появление однородного фона.</p><p>В каждой сцене имеется зацикленная анимация. Далее любую зацикленную анимацию будем называть <strong>«фоновая анимация»</strong> — не путать с анимацией фона.</p><p>Подробное описание анимации 3D ниже в соответствующем разделе.</p><h5 id="razdeli">Разделы</h5><p>В каждом разделе имеется Заголовок и краткое сообщение.</p><h5 id="1.--razdel-«nachalo».">1. Раздел «Начало».</h5><p>Название конкурса, даты проведения и краткое описание. В сноске с дополнительной информацией.</p><p><img src="images/MacBookPro-4.png" alt=""></p><h5 id="2.-razdel-«istoriya».">2. Раздел «История».</h5><p>История об основателе компании, который завещал отправить в путешествие его мечты тех, кто угадает, куда он мечтал съездить, но так и не смог.</p><p>История в десктопной версии разделена на 4 главы-слайда, в мобильной — на 8 слайдов.</p><p><img src="images/MacBookPro-1.png" alt=""><img src="images/iPhoneSE-3.png" alt=""></p><p>Остальные слайды истории:
<img src="images/MacBookPro-14.png" alt=""></p><p><img src="images/MacBookPro-15.png" alt=""></p><p><img src="images/MacBookPro-16.png" alt=""></p><p>Смена слайдов реализуется с помощью библиотеки <code>Swiper</code>. Стандартная смена слайдов отключена, реализацию смены контента нужно реализовать на смене классов и <code>CSS transition</code>.</p><p>Переход между главами синхронизируется с 3D иллюстрации на фоне: 1 слайд — 1 сцена 3d в десктопной версии, 2 слайда — 1 сцена 3D — в мобильной.</p><p>Раздел состоит из 4 сцен (экранов), по которым путешествует Чемодан. Перемещение между сценами происходит поворотом относительно одной оси.</p><h5 id="3.-razdel-«prizi».">3. Раздел «Призы».</h5><p>Кроме заголовка и текста имеется перечень призов с указанием их количества. 3 главных, 7 второстепенных и 900 утешительных. У каждого типа призов анимированная иллюстрация в <code>SVG</code>.</p><p><img src="images/MacBookPro-5.png" alt=""></p><h5 id="4.-razdel-«pravila».">4. Раздел «Правила».</h5><p>Кроме заголовка и текста имеется список шагов в игре. Внизу, в сноске, ссылки на подробные правила и правовые документы.</p><p><img src="images/MacBookPro-6.png" alt=""></p><h5 id="5.-razdel-«igra».">5. Раздел «Игра».</h5><p>Смотрите описание механики выше.</p><p>В выданной верстке встроены три кнопки для тестирования экранов результатов игры. По нажатию на эти кнопки происходит переход на экран соответствующего результата без прохождения игры. По завершении работы над анимацией экранов результатов необходимо удалить/скрыть тестовые кнопки.</p><p><figure><img src="images/MacBookPro-10.png" alt="Экраны результатов" title="Экраны результатов"><figcaption>Экраны результатов</figcaption></figure></p><p><figure><img src="images/MacBookPro-8.png" alt="Экраны результатов" title="Экраны результатов"><figcaption>Экраны результатов</figcaption></figure></p><p><figure><img src="images/MacBookPro-9.png" alt="Экраны результатов" title="Экраны результатов"><figcaption>Экраны результатов</figcaption></figure></p><h3 id="razrabotka-animatsii">Разработка анимации</h3><p>На свёрстанной странице лендинга необходимо реализовать анимацию в соответствии с видео проекта.
В отдельных случаях когда важно воспроизвести тайминг движения, в дополнении к ТЗ (в отдельных заданиях) приведены графики и описания, по которым нужно задать <strong>временные функции</strong> или <strong><code>easing</code></strong>.</p><p>Если задание никак не может быть выполнено с той версткой, которая дана верстальщиками, необходимо доработать верстку. Делать это нужно только в том случае, если вы рассмотрели все возможные варианты с текущей версткой.</p><p>В разделе 3D кроме анимации необходимо выполнить загрузку объектов и нарисовать фигуры из примитивов по схемам. Схемы будут в приложении к ТЗ (в отдельных заданиях). Временные функции будут указаны или будут приведены графики, по которым нужно воспроизвести анимацию.</p><p><strong>Замечания:</strong></p><p>Обращайте внимание на то, что анимация появления элементов в большом числе случаев отличается от анимации скрытия этих элементов.</p><h3 id="css-perekhodi-mezhdu-sostoyaniyami">CSS переходы между состояниями</h3><p><code>CSS transition</code> — для линейных переходов между состояниями.
Удобно также использовать <code>CSS variables</code> и спец.слово <code>currentColor</code> — для удобства управления, особенно при смене <strong>«темы»</strong> — <strong>«цветовой схемы»</strong>.</p><h5 id="1.-sostoyaniya-interaktivnikh-elementov.">1. Состояния интерактивных элементов.</h5><p>К интерактивным элементам относятся элементы с состояниями взаимодействия <code>hover</code>, <code>focus</code> и <code>active</code>: ссылки и кнопки.</p><p>Необходимо дополнить стили описанием анимации переходов.</p><p><img src="images/States.png" alt=""></p><h5 id="2.-otkritie-i-zakritie-knopok-sheringa-v-sotsialnikh-setyakh.">2. Открытие и закрытие кнопок шеринга в социальных сетях.</h5><p>Кнопки «подтягиваются» снизу из прозрачности.</p><p><strong>Обратите внимание</strong>, что анимация появления кнопок отличается от анимации скрытия.</p><p>Анимацию кнопок нужно сделать внахлёст по отношению друг к другу: от первого пункта к последнему. Время появления последних больше первых — <strong>эффект «первые подтягивают за собой последующие»</strong>.</p><h5 id="3-.-poyavlenie-i-skritie-kontenta-razdelov.">3. Появление и скрытие контента разделов.</h5><p><code>CSS transition</code> DOM элементов страницы — лёгкое управление при прокрутке.</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-1" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-1">1.</a> Появление заголовков и даты проведения конкурса.<br><em>Референс:</em></p><p><a href="https://artisantalent.com/for-talent/">https://artisantalent.com/for-talent/</a></p><p>Необходимо:
— — Написать скрипт, который разделит текст заголовков на символы;
— — Реализовать <code>CSS transition</code> появления каждого символа при смене класса экрана на видимый;
— — При скрытии экрана анимации быть не должно.</p><p>##### Замечание по технологии</p><p>Автоматизация разбиения текста на элементы — слова и символы — с помощью JS с учетом разметки.</p><p>Плюс автоматизация задания свойств <code>transition-duration</code>, <code>transition-delay</code>, <code>animation-duration</code>, <code>animation-delay</code> с помощью JS. Практика анимации большого количества однородных элементов в составе группы — создание общего <code>timeline</code> в CSS.</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-2" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-2">2.</a> Появление текстов в разделах.<br>
Текст появляется с задержкой после заголовка (смотрите видео).
— — Из прозрачности;
— — Снизу.</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-3" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-3">3.</a> Появление текстов в слайдере в разделе «История».<br>
В активном слайде тексты появляются справа из прозрачности (смотрите видео). Второй абзац справа появляется с задержкой и с большей длительностью по сравнению с первым абзацем.</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-4" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-4">4.</a> Появление однородного фона в разделах «Призы», «Правила», «Игра»
Реализовать появление/скрытие однородного фона в разделах снизу экрна при переходах между экранами. </p><p>Если имеющаяся верстка не позволяет реализовать анимацию в необходимом виде, нужно доработать верстку.</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-5" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-5">5.</a> Появление нумерованного списка в разделе «Правила».<br>
Пункты списка начинают появляться по очереди до того, как предыдущий элемент появился и остановился полность — <strong>«внахлёст»</strong>.
Круг появляется из центра до размера чуть больше конечного, затем переходит к конечному размеру: проскакивает по инерции конечное состояние, потом как на резинке встает в нужное положение. Движение должно показывать эластичность круга, как мячика.</p><p>Цифры анимируются отдельно и появляются из прозрачности. С появлением круга «внахлёст». Когда круг завершает движение, цифры уже появились.</p><p>Текст выезжает из прозрачности справа. Анимацию текстов пунктов нужно сделать внахлёст по отношению друг к другу: от первого пункта к последнему. Время появления последних больше первых — <strong>эффект «первые подтягивают за собой последующие»</strong>.</p><p><img src="images/MacBookPro-6.png" alt=""></p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-6" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-6">6.</a> Появление пагинации.<br>
Текст пагинации появляется быстро из прозрачности. Кнопки выезжают с двух сторон с вращением как у колеса (без проскальзывания).</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-7" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-7">7.</a> Появление кнопки «Погнали» и формы игры.<br>
У кнопки «Погнали» сначала появляется фон — вытягивается из круга. Потом до окончания движения внахлёст появляется текст. Текст не меняет размер и не движется.</p><p>При переходе к игре название кнопки «Погнали» меняется на «Узнать» через прозрачность.</p><p>В мобильной версии на кнопке стрелка вместо надписи «Узнать». Поэтому нужно сделать обратную анимацию из вытянутого фона в круг и показать стрелку.</p><p>Одновременно мгновенно появляется другой круг и вытягивается в фон поля ввода. Появляется из прозрачности <code>placeholder</code> поля.</p><p><img src="images/MacBookPro-18.png" alt=""></p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-9" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-9">8.</a> Появление ответов в чате.<br>
Вопрос быстро появляется внизу чата и отъезжает вверх на высоту поля ответа. Появляется поле ответа со спиннером, потом спиннер мгновенно исчезает и из прозрачности быстро появляется ответ.</p><p>Когда в чате уже есть сообщения нужно создать элементы, с помощью JS узнать высоту нового вопроса и ответа и поднять все предыдущие сообщения на эту высоту, затем вставить новые вопрос/ответ (анимацию здесь та же, что описана выше).</p><p>Нужно реализовать анимацию подъёма предыдущих сообщений с <strong>эффектом «первые подтягивают за собой последующие»</strong> в соответствии с видео.</p><p><img src="images/MacBookPro-19.png" alt=""></p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-9" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-9">9.</a> Появление кнопки «Не сдавайся!».<br>
Текст появляется из прозрачности. Круг со стрелкой выезжает справа с вращением как колесо. Важно сделать эту анимацию без «проскальзывания колеса».</p><p><img src="images/MacBookPro-10.png" alt=""></p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-10" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-10">10.</a> Появление/скрытие сноски.<br>
Появляется снизу и скрывается вниз без изменений прозрачности. При переходе между разделами «Призы» и «Правила». Сноска не исчезает, на ней меняется текст через прозрачность.
<img src="images/Disclaimer.png" alt=""></p><p>В мобильной версии сноска скрыта в левый нижний угол: текст скрыт в прозрачность, фон сдвинут влево вниз. При клике на звездочку выезжает фон с кнопкой скрытия и появляется текст через прозрачность.</p><p><img src="images/iPhoneSE-1.png" alt=""></p><p>Если фон выполнен свойством <code>background</code> его необходимо выделить в отдельный псевдоэлемент только в мобильной версии.</p><p><img src="images/iPhoneSE-21.png" alt=""></p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov." id="3-.-poyavlenie-i-skritie-kontenta-razdelov.">11.</a> Скрытие разделов.<br>
Все разделы кроме экрана игры исчезают через прозрачность как один слой (без анимации отдельных элементов). Кроме этого все разделы скейлятся: начало увеличивается (мы проваливаемся в замочную скважину), остальные уменьшаются.</p><p>При переходе к призам 3D сцена закрывается оверлеем-фоном фиолетового цвета. Оверлей появляется снизу.</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-12" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-12">12.</a> Скрытие экрана игры при переходе к результату игры.<br>
При переходе к результатам заголовок уезжает с прозрачностью влево, таймер — вправо, а форма переписки вниз. Чат исчезает через прозрачность.</p><p><a href="#3-.-poyavlenie-i-skritie-kontenta-razdelov.-13" id="3-.-poyavlenie-i-skritie-kontenta-razdelov.-13">13.</a> Появление текстов результатов победы.<br>
Тексты появляются с уменьшением: у заголовка больший скейл, у текста меньше. Текст появляется из прозрачности.
Заголовок рисуется обводка — смотри SVG.</p><h5 id="4-.-smena-temi-v-glavakh-istorii">4. Смена темы в главах Истории</h5><p>Необходимо реализовать смену темы элементов UI всего сайта при переходе между главами.</p><ul><li>— Добавить присвоение классов;</li><li>— Описать цвета тем;</li><li>— Передать цвета в необходимые элементы UI.</li></ul><p><img src="images/Themes.png" alt=""></p><h3 id="css-animatsiya-illyustratsii">CSS анимация иллюстрации</h3><h5 id="1.-animatsiya-tochek-spinnera-v-rezhime-ozhidaniya-otveta-bota.">1. Анимация точек спиннера в режиме ожидания ответа бота.</h5><p>Нужно сделать зацикленную анимацию точек: меняется прозрачность от 100% до 20% и обратно. Анимация трёх точек запускается с задержкой относительно друг друга — создается эффект волны.</p><h5 id="2.-animatsiya-ii-«soni»-na-ekrane-«igra».">2. Анимация ИИ «Сони» на экране «Игра».</h5><p>Необходимо сделать анимацию картинки ИИ «Сони»: как она выезжает по диагонали с вращением и скейлом. После этого картинка колеблется вверх-вниз на месте. Исчезать «Соня» должна с обратной анимацией.</p><h5 id="3.-animatsiya-illyustratsii-«chemodan-i-flamingo».">3. Анимация иллюстрации «Чемодан и фламинго».</h5><p>Необходимо сделать анимацию появления в соответствии с видео:</p><ul><li>— Чемодан движется по диагонали со скейлом из прозрачности;</li><li>— Фламинго по другой диагонали без скейла;</li><li>— Листья появляются с вращением.</li></ul><p>Нужно сделать фоновую анимацию колебания фламинго. При этом фламинго вращается относительно точки пересечения лап. Вращение идёт с небольшой задержкой относительно колебания вверх-вниз — так как происходит по инерции от этого колебания.</p><h4 id="animatsiya-tsifr-v-razdele-prizi">Анимация Цифр в разделе Призы</h4><p>Анимация цифр (количество призов) — покадровая анимация по <code>requestAnimationFrame</code>. Меняется текст, большое количество символов перебирается для эффекта, они не несут основную информацию, поэтому имеет смысл создавать временные элементы и записывать в них временные цифры с помощью JS.</p><p>Число 900 нужно начинать показывать с числа 11.</p><p>Обратите внимание, что менять цифры нужно 12 кадров в секунду. Длительность смены одного числа меньше секунды.</p><h4 id="animatsiya-taimera">Анимация Таймера</h4><p>Анимация обратного отсчета. Покадровая анимация по <code>requestAnimationFrame</code>: в кадре проверяются текущие данные объекта <code>Date</code> для показа актуальной информации о пройденном времени: обратный отсчёт с момента захода в сессию игры. Максимальная длительность одной игровой сессии — 5 минут. При повторном заходе в новую сессию игры, таймер сбрасывается. Форматирование: оставшееся время до конца сессии время округляется до меньшего и показывается в формате <code>MM:SS</code>.</p><h4 id="animatsiya-v-svg">Анимация в SVG</h4><h5 id="1-.-animatsiya-risovaniya-zagolovkov-rezultatov.">1. Анимация рисования заголовков Результатов.</h5><p>Необходимо сделать анимацию рисования контуров заголовков результатов игры. Обратите внимание, что рисуется из двух-трех точек одновременно.</p><p>Символы «Не угадал!» при этом должны падать сверху с одним отскоком.</p><p>Все символы «Победа!» появляются одновременно, а символы «Не угадал!» должны появляться с задержкой внахлёст. Обратите внимание на движение контура, которых создают символы вместе: он изогнутый, не прямой.</p><h5 id="2-.-animatsiya-illyustratsii-prizov.">2. Анимация иллюстраций призов.</h5><p>SMIL-анимация в SVG. Анимация изолируется в SVG, начало сюжета проигрывается один раз, фоновая анимация остается и зацикливается.
Необходимо обратить внимание на следующие нюансы анимации SVG:</p><ul><li>— Движение вдоль <code>path</code>;</li><li>— Способы задания центра трансформации, так как css-свойство <code>transform-origin</code> поддерживается по-разному в разных браузерах и как правило, задаётся относительно всего SVG, а не относительно элемента;</li><li>— Позволяет морфить <code>path</code>.</li></ul><p>Для каждой иллюстрации даётся по два SVG файла: начальное и конечное состояние картинок.</p><p><img src="images/SVGAnimationStart.png" alt=""></p><p><img src="images/SVGAnimation.png" alt=""></p><p><a href="#2-.-animatsiya-illyustratsii-prizov.-1" id="2-.-animatsiya-illyustratsii-prizov.-1">1.</a> Анимация дирижабля.</p><p>Летит дирижабль, покачиваясь. В дирижабле одно из окошек приближается и становится большим, к окошку подъезжает кресло, лыжи и лист.</p><p><strong>Фоновая анимация:</strong> в окошке летят облака, лыжи и листок покачиваются.</p><p><em>Референс:</em></p><p><a href="https://dribbble.com/shots/3002580-Dirigible-animation">https://dribbble.com/shots/3002580-Dirigible-animation</a> — полет дирижабля, амплитуду сделать небольшой;</p><p><a href="https://dribbble.com/shots/7440664-Illustration-for-a-Travel-Reward-Credit-Card-Service-Website">https://dribbble.com/shots/7440664-Illustration-for-a-Travel-Reward-Credit-Card-Service-Website</a> — облака в окне.</p><p><a href="#2-.-animatsiya-illyustratsii-prizov.-2" id="2-.-animatsiya-illyustratsii-prizov.-2">2.</a> Анимация чемодана с парашютом.</p><p>Появляется облако, из облака выпадает парашют с чемоданом, приземляется в растения, облака улетают вверх с прозрачностью.</p><p><strong>Фоновая анимация:</strong> листья колеблются и облака передвигаются.</p><p><em>Референс:</em></p><p><a href="https://dribbble.com/shots/4111276-Up-in-the-Clouds">https://dribbble.com/shots/4111276-Up-in-the-Clouds</a> — траектория проще.</p><p><a href="#2-.-animatsiya-illyustratsii-prizov.-3" id="2-.-animatsiya-illyustratsii-prizov.-3">3.</a> Анимация чемодана с воздушным шариком.</p><p>Появляется чемодан из прозрачности, открывается крышка, из чемодана поднимается воздушный шарик на веревочке, веревочка не даёт шарику улететь — шарик колеблется и останавливается. Одновременно появляются цветы, и рядом колибри.</p><p><strong>Фоновая анимация:</strong> колибри летает.</p><p><em>Референсы:</em></p><p><a href="https://dribbble.com/shots/4028029-Travel-Insurance">https://dribbble.com/shots/4028029-Travel-Insurance</a>.</p><h4 id="animatsiya-illyustratsii-v-canvas">Анимация иллюстраций в Canvas</h4><p>Необходимо повторить анимации иллюстраций результатов игры проигрыша и выигрыша главного приза из видео-примера.</p><p>По завершении работы над анимацией результатов необходимо удалить/скрыть тестовые кнопки показа результатов.</p><p><strong>Замечание по технологии</strong>
Использовать нужно низкоуровневое рисование в canvas с помощью JS.</p><h5 id="1-.-animatsiya-s-morzhom.">1. Анимация с моржом.</h5><p>Необходимо сделать рисование в canvas:</p><ul><li>— Всплытие моржа на льдине — воспроизвести затухающие колебания вверх-вниз и вращения как в видео;</li><li>— Появление снежинок и фоновую анимацию колебания снежинок вверх/вниз;</li><li>— Вылет самолета по части синусоиды (наклон самолета соответствует положению на синусоиде);</li><li>— Рисование следа от самолета (cubic-bezier+круг), точка и наклон остного конца совпадает с хвостом самолета, круглый конец — круг, который увеличивается на одном месте (верхний край закреплен).</li></ul><h5 id="2-.-animatsiya-s-krokodilom.">2. Анимация с крокодилом.</h5><p>Необходимо сделать рисование в canvas:</p><ul><li>— Появление замочной скважины из прозрачности;</li><li>— Вылет объектов из центра и падение их вниз за край экрана: они должны сначала зависнуть, а затем, с ускорением улететь вниз;</li><li>— Появление из-за маски крокодила.</li></ul><p><strong>Фоновая анимация:</strong> капают слезы из глаза крокодила. 1 слеза — 1 цикл.</p><h4 id="animatsiya-3d-illyustratsii">Анимация 3D-иллюстрации</h4><p>Из предоставленных материалов необходимо собрать сцены в 3D с помощью библиотеки <code>Three.JS</code> в соответствии с дизайном.</p><p>При сборке сцен если не указаны точные координаты объектов, необходимо ориентироваться на внешнее сходство (для ускорения работ). По запросу может быть предоставлен исходник 3D в Cinema 4D.</p><p>Необходимо выполнить:</p><ul><li>— Фоновые анимации на сценах;</li><li>— Переходы между сценами с помощью анимации камеры;</li><li>— Эффект реакции на движение курсора: изменение точки, откуда смотри камера;</li><li>— Растровый эффект поверх сцены с помощью техники <code>Post-Processing</code>.</li></ul><h5 id="stsena-«zamochnaya-skvazhina»">Сцена «Замочная скважина»</h5><p><a href="#stsena-%C2%ABzamochnaya-skvazhina%C2%BB-1" id="stsena-%C2%ABzamochnaya-skvazhina%C2%BB-1">1.</a> Сборка сцены из элементов.</p><p>Загружаемые объекты:</p><ul><li>— Чемодан;</li><li>— Самолет;</li><li>— Арбузная долька.</li></ul><p>Объекты, составленные из примитивов:</p><ul><li>— Планета Сатурн из сферы и диска;</li></ul><p>Геометрии Extrude из SVG:</p><ul><li>— Плоскость с замочной скважиной;</li><li>— Снежинка;</li><li>— Вопрос;</li><li>— Лист;</li><li>— Фламинго;</li></ul><p><a href="#stsena-%C2%ABzamochnaya-skvazhina%C2%BB-2" id="stsena-%C2%ABzamochnaya-skvazhina%C2%BB-2">2.</a> Анимация разлёта элементов сцены.</p><p>Появление из центра замочной скважины с изменением скейла из 0 и изменением вращения. Вращение нужно подобрать самостоятельно.</p><p><a href="#stsena-%C2%ABzamochnaya-skvazhina%C2%BB-3" id="stsena-%C2%ABzamochnaya-skvazhina%C2%BB-3">3.</a> Анимация самолета.</p><ul><li>— Самолет;</li><li>— Проходит по дуге из-за скважины;</li><li>— Огибает край скважины;</li><li>— Увеличивается в размере;</li><li>— Вращается относительно собственной оси.</li></ul><p>Рекомендуется делать после выполнения заданий по анимации камеры.</p><h5 id="4-stseni-«istoriya»">4 сцены «История»</h5><p><a href="#4-stseni-%C2%ABistoriya-1%C2%BB" id="4-stseni-%C2%ABistoriya-1%C2%BB">1.</a> Сборка сцен из элементов.</p><p>Загружаемые объекты:</p><ul><li>— Чемодан;</li><li>— Стены одной комнаты;</li><li>— Собака;</li><li>— Комната 1 — общая часть с комнатой 4;</li><li>— Комната 1 — оставшаяся часть;</li><li>— Комната 2;</li><li>— Комната 3;</li><li>— Компас;</li><li>— ИИ «Соня» в комнату 4.</li></ul><p>Объекты, составленные из примитивов:</p><ul><li>— Люстра в форме планеты Сатурн: 2 сферы, диск и цилиндр,
пирамида;</li><li>— Фонарный столб: 2 цилиндра, сфера, 3 усеченные пирамиды;</li><li>— Снеговик: 2 сферы и конус;</li><li>— Столбики у дороги.</li></ul><p>Геометрии Extrude из SVG:</p><ul><li>— Цветок в комнате 1;</li><li>— Листья в комнате 2.</li></ul><h5 id="svet:">Свет:</h5><p>Нужно поставить в соответствии со схемой, прилагающейся в архиве с объектами.</p><p><strong>Материалы:</strong>
Всем объектам нужно задать материал в соответствии со схемой, прилагающейся в архиве с объектами и SVG для загрузки.</p><p>Для мобильной версии нужно отключить свет и заменить материалы на <code>MatCap</code>. Картинки прилагаются в архиве.</p><p><a href="#4-stseni-%C2%ABistoriya-2" id="4-stseni-%C2%ABistoriya-2">2.</a> Анимация хвоста собаки в 1 сцене истории.</p><p>Необходимо сделать покадровую анимацию виляния хвоста собаки в соответствии с видео.</p><p><a href="#4-stseni-%C2%ABistoriya-3" id="4-stseni-%C2%ABistoriya-3">3.</a> Анимация покачивания люстры «Сатурн» в 1 сцене истории.</p><p>Необходимо сделать покадровую анимацию колебания люстры в соответствии с видео (без затухания). Диск должен также колебаться с задержкой относительно колебания люстры, так как это инерционное движение.</p><p><strong>Временные функции:</strong> можно использовать синусоиду.</p><p><a href="#4-stseni-%C2%ABistoriya-4" id="4-stseni-%C2%ABistoriya-4">4.</a> Анимация листьев в 2 сцене истории.</p><p>Необходимо сделать покадровую анимацию колебания листьев в соответствии с видео.
Колебания должны быть с затуханием и возобновляться через некоторый промежуток времени.</p><p><strong>Временные функции:</strong> можно использовать синусоиду.</p><p><a href="#4-stseni-%C2%ABistoriya-5" id="4-stseni-%C2%ABistoriya-5">5.</a> Анимация стрелки в 3 сцене истории.</p><p>Необходимо сделать покадровую анимацию колебания листьев в соответствии с видео.</p><p><strong>Временные функции:</strong> похожа на синусоиду, но более пологая в крайних точках. График будет приложен в заданиях.</p><p><a href="#4-stseni-%C2%ABistoriya-6" id="4-stseni-%C2%ABistoriya-6">6.</a> Анимация флуктуации ИИ «Сони».
Необходимо сделать покадровую анимацию колебания «Сони» вверх/вниз в соответствии с видео. Нужно сделать колебания рук «Сони» с задержкой относительной колебания «Сони», так как это инерционное движение.</p><p><strong>Временные функции:</strong> можно использовать синусоиду.</p><h4 id="animatsiya-kameri">Анимация камеры</h4><p>Для анимация переходов между сценами и реакция на движение курсора необходимо использовать технику <code>Rig</code> Камеры.</p><p>Необходимо сделать конструкцию для пролета в замочную скважину и облёта вокруг сцен с комнатами. Далее нужно реализовать анимацию с помощью рига.</p><p>В конструкции рига нужно учесть то, что камеру нужно вращать вверх/вниз относительно центра сцены при движении курсора. Смотри пример в видео.</p><p><em>Референс:</em></p><p><a href="https://www.instagram.com/p/B6dfJOaBBUi/?igshid=12zvwose8z2ce">https://www.instagram.com/p/B6dfJOaBBUi/?igshid=12zvwose8z2ce</a>.</p><p>С помощью настроек камеры и рига нужно реализовать изменение отображения сцен при портретной ориентации сайта.</p><h4 id="rastrovaya-animatsiya-poverkh-3d-stseni-«bliki-i-puziri»">Растровая анимация поверх 3D-сцены «Блики и пузыри»</h4><p>Использовать необходимо <code>Post-Processing</code>.</p><p>Однако вставлять два контекста <code>WebGL</code> — большая нагрузка на браузер. На слабых устройствах это может привести к прекращению работы браузера.
При <code>Post-Processing</code> можно использовать шейдеры 2D эффектом поверх 3D сцен.</p><p>Необходимо сначала работать с картинкой из макета для написания шейдера для 2D-эффекта, а затем перенести эти шейдеры на canvas с 3D.</p><p>Описание эффекта:</p><ol><li>Небольшое колебание <code>Hue</code> цвета, с достижением эффекта легкого мерцания.</li><li>Три круглых линзы — картинка расширена по центру и сжата по краю круга — двигаются по затухающей синусоиде снизу вверх.</li><li>Вокруг линз 2-пиксельная полупрозрачная обводка и один сектор круга в левом верхнем крае круга внутри — блик.</li></ol></div></div></div></div></div><button class="up-interface__chat-control" type="button" title="Свернуть"><span class="sr-only">Свернуть</span><svg aria-hidden="true" width="8" height="16"><use xlink:href="/img/sprites/up.svg?cs=fb70597153879c70ce140224310b7444b664990a#icon-arrow-right"></use></svg></button>
