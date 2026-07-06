# Яндекс.Метрика для сайта

К сайту, созданному в Salebot, можно подключить Яндекс.Метрику. Для этого создайте счётчик в Яндекс.Метрике, создайте цели и укажите данные в настройках сайта:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.54.14.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.52.29.png" alt=""><figcaption><p>Чтобы указать ID Метрики, перейдите в настройки сайта.</p></figcaption></figure></div>

**ID Яндекс Метрики.** Укажите ID счётчика Я.Метрики

## Как создать счетчик Яндекс.Метрики?

Для начала сбора оффлайн конверсий в Яндекс.Метрику с Salebot необходимо зарегистрировать Яндекс.Метрику.

**1.** **Если у Вас нет аккаунта Яндекс.Метрики**, следует войти в ваш аккаунт Яндекс почты (или зарегистрировать новый). Далее перейти в[ Яндекс.Метрику](https://metrika.yandex.ru/list?) и нажать добавить счетчик.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.06.49.png" alt="" width="375"><figcaption></figcaption></figure></div>

В настройках счетчика указать следующие данные:

1. Имя счетчика
2. Адрес сайта - в примере ссылка на сайт Salebot (и далее пример будет построен на нем).

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.08.48.png" alt="" width="563"><figcaption><p>Домен или путь без https, http, www</p></figcaption></figure></div>

4. Автоматические цели и Вебвизор, карта скроллинга и аналитика форм - рекомендуем включить обе галочки для сбора большего количества информации.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.11.28.png" alt="" width="563"><figcaption></figcaption></figure></div>

После заполнения страницы жмем “Создать счетчик”.

## Как вставить счетчик Метрики на сайт для оффлайн-конверсий?

После создания счетчика, на открывшейся странице скопируйте html-код, появившийся внизу. Затем нажимаем кнопку “Начать пользоваться”.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.12.56.png" alt=""><figcaption></figcaption></figure></div>

Если у вас уже есть счетчик, то найти код счетчика вы сможете в настройках:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.24.54.png" alt=""><figcaption></figcaption></figure></div>

Далее перейдите в настройки сайта в Salebot:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.52.29.png" alt=""><figcaption><p>Чтобы вставить HTML-код счетчика, перейдите в настройки сайта.</p></figcaption></figure></div>

В настройках сайта во вкладке “Настройки” раздел “HTML” добавьте код в поле HTML-код head(или HTML-код body):

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.14.16.png" alt=""><figcaption></figcaption></figure></div>

Далее нажмите "Сохранить".

Перейдите в Метрику и найдите ID счетчика: скопирейте его:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.15.53.png" alt=""><figcaption></figcaption></figure></div>

Далее в Salebot перейдите в настройки проекта и создайте константу проекта ym\_counter\_id:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.17.26.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.18.30.png" alt=""><figcaption></figcaption></figure></div>

**2. Если у Вас есть аккаунт в Яндекс Метрике**, то следует зайти в счетчик, по которому Вы хотите собирать статистику и записать его номер в переменную проекта ym\_counter\_id (настройки проекта - константы проекта). Настраивать счетчик заново Вам не нужно, просто вносим переменную как показано на скриншоте выше и переходим сразу к следующему пункту.

## Как подключить Яндекс.Метрику по ID?

{% hint style="success" %}
Для подключения Метрики необходимо в поле вписать ID Яндекс Метрики.&#x20;
{% endhint %}

В поле ID Яндекс метрики указывается ID счетчика Яндекс Метрики: его вы можете увидеть на странице Яндекс Метрики в разделе “Обзор” вверху возле Имени счетчика и Адреса сайта:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.04.43.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="success" %}
Вставка ID счетчика равносильна добавлению “[Код счетчика](yandeks.metrika-dlya-saita.md#kak-vstavit-schetchik-metriki-na-sait-dlya-offlain-konversii)” на сайт
{% endhint %}

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.54.14.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.52.29.png" alt=""><figcaption><p>Чтобы указать ID Метрики, перейдите в настройки сайта.</p></figcaption></figure></div>

**ID Яндекс Метрики.** Укажите ID счётчика Я.Метрики

## Настройка целей

Далее вам следует создать цель/цели на сайте Яндекс Метрики.&#x20;

Шаг 1. Перейдите в раздел “Цели” и нажмите кнопку “Добавить цель”. У вас откроется меню для создания новой Цели.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.08.05.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.09.05.png" alt=""><figcaption></figcaption></figure></div>

Шаг 2. Выберите целевое событие: “JS-событие”.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.09.39.png" alt=""><figcaption></figcaption></figure></div>

Откроется вкладка, где нужно прописать название цели и идентификатор:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.11.28.png" alt="" width="563"><figcaption></figcaption></figure></div>

В поле “Идентификатор цели” нужно прописать идентификатор, который вы позже укажите в настройках сайта. В поле “Название” вы можете написать что угодно.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.13.22.png" alt="" width="563"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Цель будет срабатывать по нажатию на любую кнопку на сайте.
{% endhint %}

{% hint style="success" %}
Если вы хотите разделить цели по нажитию на разные кнопки минилендинга, название цели должно заканчиваться на знак подчеркивания "\_"
{% endhint %}

Пример:\
Если вы передадите в наше поле “click\_button”, тогда вам в Яндекс Метрику будет передаваться одна Цель по клику на любой из мессенджеров.&#x20;

Цель с идентификатором “click\_button”.\
Однако, если вы передадите в наше поле “click\_button\_” (у которого в конце стоит “\_” знак нижнего подчеркивания), в вашу Яндекс.Метрику будет передаваться разная цель для разного мессенджера,

{% hint style="danger" %}
\*Facebook, WhatsApp, Instagram принадлежат Meta platform Inc., деятельность которой признана в РФ экстремистской и запрещена.
{% endhint %}

click\_button\_0 - по клику на ВКонтакте\
click\_button\_1 - по клику на Телеграм\
click\_button\_2 - по клику на Viber\
click\_button\_3 - по клику на FaceBook\*\
click\_button\_6 - по клику на WhatsApp\*\
click\_button\_8 - по клику на Одноклассники\
click\_button\_10 - по клику на Instagram\*\
click\_button\_20 - по клику на MAX

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.15.55.png" alt=""><figcaption></figcaption></figure></div>

Сам идентификатор может быть любой. Главное, чтобы в конце было нижнее подчеркивание. К нему будет добавлен индекс мессенджера.

Пример правильно заполненных полей в настройках сайта и правильно созданных целей в Яндекс Метрике:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.16.53.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 15.17.52.png" alt=""><figcaption></figcaption></figure></div>

Для настройки события для кнопки, перейдите в настройки кнопки.

## Настройка событий по кликам на кнопку

Чтобы отследить события по заявкам и(или) переходам в бота с сайта, вам нужно перейти в настройки сайта, в котором создана форма отправки заявки или с кнопками на мессенджеры:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-04-09 в 16.00.31.png" alt=""><figcaption></figcaption></figure></div>

Далее наведите на блок "Форма" и найдите кнопку "Настройки":

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-04-09 в 16.01.49.png" alt=""><figcaption></figcaption></figure></div>

Раскройте настройки кнопок:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-04-09 в 16.02.33.png" alt=""><figcaption></figcaption></figure></div>

Здесь вы увидите поле, где нужно вставить название события, настроенное в Яндекс Метрике:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-04-09 в 16.03.36.png" alt="" width="563"><figcaption></figcaption></figure></div>

Чтобы отправка событий работала, [нужно вставить скрипт счетчика Метрики на сайт.](yandeks.metrika-dlya-saita.md#kak-vstavit-schetchik-metriki-na-sait-dlya-offlain-konversii)

Аналогично можно проставить название событий для каждой кнопки мессенджера.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-04-09 в 16.06.55.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-04-09 в 16.07.28.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-04-09 в 16.07.47.png" alt="" width="375"><figcaption></figcaption></figure></div>

## Как передать данные в Яндекс.Метрику?

{% hint style="warning" %}
**ВАЖНО!**

Отправка оффлайн-конверсий происходит по идентификатору клиента Яндекс. Если у клиента в переменных есть метка \_ym\_uid ([как включить сбор меток в минилендингах смотрите в соответствующем разделе](../../websites/builder/analitika-saita.md)), он автоматически подставится в этот параметр и передаст статистику по данному клиенту.&#x20;

С момента запуска бота до передачи офлайн-конверсии должно пройти достаточно времени для передачи метки \_ym\_uid в Метрику, например, от 5-10 минут.
{% endhint %}

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.21.24.png" alt="" width="563"><figcaption></figcaption></figure></div>

\_ym\_uid - это client ID посетителя, присваиваемый Яндексом каждому пользователю. Он является уникальным и задается только системой Яндекс. Поэтому, если у клиента нет параметра, статистика по нему передаваться не будет. Однако, если у Вас есть данные о метке посетителя, Вы можете добавить клиенту переменную ya\_client\_id, и, если такой посетитель существует, статистика передастся.&#x20;

{% hint style="info" %}
Если клиента с номером, указанным в ya\_client\_id, не существует, то и статистика собираться не будет&#x20;
{% endhint %}

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (492).png" alt=""><figcaption></figcaption></figure></div>

Если посетитель с меткой \_ym\_uid прошел по этапам, статистика соберется и отправится в Яндекс Метрику, где потом будет обработана. Статус обработки до появления информации в статистике можно посмотреть в счетчике - настройки -загрузка данных.

{% hint style="warning" %}
**Внимание!**

Обработка может длиться до 24 часов! По итогу, при успешной загрузке появится значок “Выполнено”, при неуспешной - красная надпись. Это означает, что Яндекс Метрика не обнаружила клиента по заданному \_ym\_uid в своей системе.
{% endhint %}

Для работы с функцией нам понадобится токен. Для этого нужно перейти в кабинет Метрики в Яндексе в раздел Счетчик в настройках:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.38.08.png" alt=""><figcaption></figcaption></figure></div>

Далее пролистните вниз и найдите вкладку "Дополнительные настройки" и разверните ее:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.37.11.png" alt=""><figcaption></figcaption></figure></div>

Разверните вкладку "Безопасность и использование данных" и найдите графу "Measurement Protocol":

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.37.37.png" alt=""><figcaption></figcaption></figure></div>

Отметьте галочкой "Measurement Protocol", чтобы скопировать токен:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.41.59.png" alt=""><figcaption></figcaption></figure></div>

Токен нужно сохранить в переменную проекта ym\_measurement\_token.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-23 в 16.43.43.png" alt=""><figcaption></figcaption></figure></div>

### Функция для передачи данных в Яндекс.метрику

ym\_event(event, client\_id\_type, page\_url, counter\_id, measurement\_token) - передача данных в Яндекс метрику

параметры:

<table><thead><tr><th width="267.3515625">Параметры</th><th>Описание</th></tr></thead><tbody><tr><td><mark style="color:$danger;"><strong>!</strong></mark> event </td><td>событие, которое нужно отправить в аналитику (идентификатор цели). Обязательный параметр</td></tr><tr><td>client_id_type</td><td>позволяет использовать по выбору yclid или _ym_uid для идентификации пользователя. Для использования yclid в этом параметре передайте 'yclid', во всех иных случаях будет отрабатывать как раньше. Необязательный параметр</td></tr><tr><td>page_url</td><td>адрес сайта. Параметр обязательный, если в настройках счетчика включена функция "Принимать данные только с указанных адресов".</td></tr><tr><td>counter_id</td><td>номер счетчика. Нужно указать, если в проекте ведется работа с несколькими счетчиками. Если не передан, будет взят из переменной проекта ym_counter_id</td></tr><tr><td>measurement_token</td><td>Секретный токен, генерируется при включении опции Measurement Protocol. Нужно указать, если в проекте ведется работа с несколькими счетчиками. Если не передан, будет взят из переменной проекта ym_measurement_token</td></tr></tbody></table>

{% hint style="warning" %}
Важно!

measurement\_token и counter\_id  в параметрах функции  приоритетнее тех, что указаны в настройках проекта.
{% endhint %}
