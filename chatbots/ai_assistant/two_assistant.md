# Как создать 2-х и более ассистентов в одном чате

Для комбинированной работы ассистентов нам понадобится конструктор воронок и три аи-ассистента: блоки в конструкторе понадобятся для присвоения переменных, которые будут прописаны в условии ассистента, тогда как сами ассистенты будут выступать в роли консультантов для клиента.&#x20;

Будет создано три ассистента со следующими ролями:

1. Ассистент-распределитель;
2. Менеджер по продажам
3. Бухгалтер

## Работа в конструкторе

Нам понадобятся три блока в конструкторе воронок - все блоки должны быть “Не состояние”.&#x20;

Блоки Не состояния играют следующую роль:

1. В них вложены переменные, которые будут присвоены клиенту со значением 1 или 0;
2. В первом блоке "Не состояние" будет вызываться ассистент-распределитель
3. В  первом блоке будут обнуляться переменные для дальнейшего переключения с одного ассистента на другого.&#x20;

В первом блоке назначаем переменные в калькуляторе со значением 0:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 18.02.07.png" alt=""><figcaption></figcaption></figure></div>

Код из калькулятора:

`bookeeper = 0`\
`salesman = 0`

Также пропишите необходимое сообщение в блоке.&#x20;

Во втором блоке, который будет вызван ассистентом по команде, устанавливаем значение переменной booker = 0, saleman = 1:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 18.02.52.png" alt=""><figcaption></figcaption></figure></div>

Код из калькулятора:

`bookeeper = 0`\
`salesman = 1`

В третьем блоке устанавливаем значения переменных bookeeper = 1, salesman = 0:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 18.03.17.png" alt=""><figcaption></figcaption></figure></div>

Код из калькулятора:

`bookeeper = 1`\
`salesman = 0`

Настройка блоков завершена.&#x20;

## Настройка трех АИ-ассистентов:

Создаем первого ассистента, который будет играть роль распределителя для последующих ботов с ИИ.

В настройках бота прописываем его должность, а также необходимые вводные инструкции:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 17.44.38.png" alt=""><figcaption></figcaption></figure></div>

Данный ассистент нам понадобится только для того, чтобы переключать клиента на менеджера по продажам или бухгалтера.

В разделе "Запуск команд" в настройках ассистента прописываем боту выбираем блок, в котором переменная salesman = 1 и прописываем, когда должен вызываться данный блок:

<figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 17.54.29.png" alt=""><figcaption></figcaption></figure>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 17.53.12.png" alt=""><figcaption></figcaption></figure></div>

Аналогично прописываем команду, если клиенту нужна консультация бухгалтера.

Настройки ассистента-распределителя завершены.&#x20;

#### Создаем второго ассистента - менеджера по продажам.&#x20;

Для этого кликните по кнопке для создания второго ассистента:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXcwYiPL9-l2U4caGgbRrof7FyKaElWAMTxQH1Ho1nPPJE9Ov0Ekgi0cdB9yglCokFCxcfAARnEXJNX6adB03TaNWW1R64xP5mQJ0Qz99N31DLbuc7wtjljQkV7NvULSRZCLNPCYqqKoWE1vmAyoEHiSLNBQ?key=g9-j53ENQsA_W1hDFrramA" alt=""><figcaption></figcaption></figure></div>

Можно переименовать ассистента по своему усмотрению:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXdJG_O6pJRvDgd58E9fD9Vgr30thcGl1SkBdMy3vBRpVlb73pY_yFFBeyXC6LkXH2guK0ku03ZSyN--huMHJZlRhZD2tGxHCWbGXhOYoCFSmIlJa3FLy5nDuDLczY63_a4XG9ZEj3a2agM6JGRIETF_9jDR?key=g9-j53ENQsA_W1hDFrramA" alt="" width="375"><figcaption></figcaption></figure></div>

Устанавливаем роль - продажник, а также применяем по необходимости заготовленные настройки:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXewoeYikxcZoCjdP07NhZmlIDfFc6IMs2O_2CzOstqtEEIZH2PakNnCRyl6bsD2PF3QTFdxOf2JscESONbpmKFAuSXFY23yMiHZL-sA6qTFJRXo3fa3fnMQ8dDP61CqSooXvkN5XXv4Bi4iSh830_sWlnxB?key=g9-j53ENQsA_W1hDFrramA" alt=""><figcaption></figcaption></figure></div>

В строке с условием обязательно устанавливаем переменную со значением salesman == 1:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXckPvyvI3VDWpU19-hJTIZq-9yaSZmLTkAEuTLClNowfCkhUyLtdo2aao505wXBr3yDOuMyJrPVOW5WPqxsvpnnFDYbp_IlDSnhtB6fvnkV4qoYtbo90xOoMIajAGxjSzKI1fozcv4WtyCYVoO6ER5mATLB?key=g9-j53ENQsA_W1hDFrramA" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Для чего это нужно?

Когда клиент напишет вашему распределителю, что хочет связаться с продажником, чат-бот вызовет блок, в котором содержится переменная salesman = 1, что позволит переключить клиента на бота-менеджера по продажам.&#x20;

Бот менеджера по продажам отработается только тогда, когда условие запуска будет удовлетворяться: а именно только при вызове блока, в котором переменной salesman присвоено значение 1.&#x20;
{% endhint %}

Далее переходим к настройкам бота:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 17.56.55.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="warning" %}
Важное в настройках: Необходимо обязательно прописать команды для переключения на других ассистентов с вызовом блоков из конструктора!
{% endhint %}

Настройки команд Ассистента-продажника:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 17.59.57.png" alt=""><figcaption></figcaption></figure></div>

Настройка менеджера по продажам завершена.&#x20;

#### Переходим к последнему чат-боту с ИИ - бухгалтеру.

Также создаем третьего ассистента и прописываем его название:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXeu9saJ7Z9vvMMywgWlTdE7Kn9W0x-TD9znuTgzWo-4ARZJii6aF7VBLWbxulX_9NiKYSmAc_CxvqHAkcO2vpMf-VjsPu23QWjR3MvjlXt2qDyZmwHL39uzpj8w16Q1DB7xQScXnQ1vDGJ2WatpulgT71M8?key=g9-j53ENQsA_W1hDFrramA" alt="" width="375"><figcaption></figcaption></figure></div>

В условии запуска установите переменную bookeeper == 1:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 18.05.03.png" alt=""><figcaption></figcaption></figure></div>

Условие запуска сработает только в том случае, если в вызываемом в последующем блоке будет содержатся переменная booker со значением 1.

Далее прописываем настройки ассистента:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 18.05.49.png" alt=""><figcaption></figcaption></figure></div>

Аналогично указываем команды:

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Снимок экрана 2026-06-25 в 18.06.23.png" alt=""><figcaption></figcaption></figure></div>

Настройка ассистентов завершена.&#x20;

## Тестирование работы

1. При запуске бота отработался ассистент-распределитель:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXdx86X6DsdGNm7vHd-5aX10Za0dS1CTjLNVxzowNLh3_EbN-wUD_D27qQXoW8F6-U4bRhrC15ENOpYDfp9V7IDsz-IDT3tzN0KxVAC2HXWaw-Hjfwml4I3b2dArxBAxZvsA6AmXRNKbNEs-N9RjYvDLU6pr?key=g9-j53ENQsA_W1hDFrramA" alt="" width="375"><figcaption></figcaption></figure></div>

2. Далее вызываем менеджера по продажам и видим, что подключился ассистент-продажник:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXfQ5XKyb_ANaCHk2O6kcy27lZp80TVUzkgu5a6p4YF6-o4QGsq2_bJwnwi6Qiq55NmlCwGDX77WkJbLfCQOwfk16rz4A9vUvcmJAqZ4vu5okHdX8QOWsiHP60ncAVHYHnApI2Bs3NcBhzqYrZYmxRd5ueE?key=g9-j53ENQsA_W1hDFrramA" alt="" width="375"><figcaption></figcaption></figure></div>

3.  Затем просим менеджера по продажам переключить нас на бухгалтера:<br>

    <div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXcVLcfuNURcqniMQAqDynbmduAzebMNQHNHb9HbL45tELBLXEh39GaWFQcmE1mE4_10agLBR2I8M2YMcf1iEV01hoKrCirefh_PNkGIamhpF3zl-m6wRKXoNzih02IH8kqKg4pp5GieWOaw_ZHR4SGQoVMp?key=g9-j53ENQsA_W1hDFrramA" alt="" width="375"><figcaption></figcaption></figure></div>
4. Теперь можем вернуться к ассистенту-распределителю:

<div data-with-frame="true"><figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXdh2PGlYsYnL1NLMKPtLQmn8HZ2dqsWDDp9UlcILaet_vynMhAX16VOHp8JvIOxKm112nEHCgAYNo83jwEWbJ2UTZsa5XT1dry65YrEsaES81c1LCqhCanx4f8CbofXeJ4EU1V1wVi6HzAvW-Zg20On3hs?key=g9-j53ENQsA_W1hDFrramA" alt="" width="375"><figcaption></figcaption></figure></div>

Таким образом, наш бот отработался корректно.

## Видеогид

{% embed url="https://youtu.be/KEV4_--ETuo" %}
