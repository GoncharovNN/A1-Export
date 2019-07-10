## Экспортная библиотека для систем 1С
Библиотека со многими функциями, которые могут значительно облегчить жизнь программисту 1С. Подключается как расширение (версии 8.3.12 и старше). Совместимо с любыми конфигурациями.
### Предупреждение:
Несмотря на то, что библиотека используется в продуктивных базах, её не стоит рассматривать как законченное продуктивное решение, готовое к эксплуатации в HighLoad-системах. Библиотека активно разрабатывается. Обратная совместимость предполагается, но не гарантируется. Документация библиотеки на данном этапе оставляет желать лучшего.

Некоторые встроенные функции при возникновении исключения перехватывают его и выводят пользователю сообщение с инструкцией к действию, которая вкратце сводится к "Свяжитесь с техподдержкой по этому адресу". Если Вы хотите чтобы Ваши пользователи связывались с Вами, а не со мной, необходимо переопределить процедуру "А1Э_Общее.МассивКонтактов()".

Некоторые возможности библиотеки основаны на механизмах БСП. Например, при попытке получения значения дополнительного сведения в конфигурации, не имеющей регистра "Дополнительные сведения", Вы получите исключение. Можно просто не использовать соответствующие функции.

### Возможности:
 * Значительное количество функций для работы с примитивными типами, распределенные по индивидуальным модулям.
 * Функции для удобной работы с дополнительными реквизитами.
 * Функции для работы с Ворд и Эксель.
 * Функции для работы с СКД.
 * Функции для удобного программного создания реквизитов и элементов форм.
 * И многое другое.

Файлы созданы с использованием стандартной выгрузки в xml системы 1С. Соответственно, каталог можно обратно собрать обратно в расширение с помощью конфигуратора. Альтернативно, можно использовать файл А1Э.cfe - это уже собранное расширение. 