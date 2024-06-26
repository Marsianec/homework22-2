# Домашнее задание к занятию «Микросервисы: принципы» - Тертерян Вячеслав

---

### Задание 1  

Предложите решение для обеспечения реализации API Gateway. Составьте сравнительную таблицу возможностей различных программных решений. На основе таблицы сделайте выбор решения.

Решение должно соответствовать следующим требованиям:
- маршрутизация запросов к нужному сервису на основе конфигурации,
- возможность проверки аутентификационной информации в запросах,
- обеспечение терминации HTTPS.

Обоснуйте свой выбор.  

Ответ:  

![alt text](https://github.com/Marsianec/homework22-2/blob/main/img/1.png)  

Исходя из изучение материала, и составленной таблицы, я бы выбрал для проектов на территории РФ Yandex API. Он не является угрозой попадания под санкции, так же само облако от Яндекс удобно в использование, а используя его мне кажется оптимально будет использовать современный продукт из одной линейки. Плюсом является использования сертификатов для политик безопасности и возможность взаимодействия из "коробки" с разными частями облаков от Яндекс.  

---

### Задание 2  

Составьте таблицу возможностей различных брокеров сообщений. На основе таблицы сделайте обоснованный выбор решения.

Решение должно соответствовать следующим требованиям:  
- поддержка кластеризации для обеспечения надёжности,
- хранение сообщений на диске в процессе доставки,
- высокая скорость работы,
- поддержка различных форматов сообщений,
- разделение прав доступа к различным потокам сообщений,
- простота эксплуатации.  

Обоснуйте свой выбор.  

Ответ:  

![alt text](https://github.com/Marsianec/homework22-2/blob/main/img/2.png)  

Брокеров сообщения на самом деле великое множество, взял три самых популярных на данный момент.
Вот тут с выбором все немного сложнее, так как зависит от задач которые данный брокер будет выполнять в нашей системе микросервисов, а так же от количества запросов в системе.
В среднем, если не смотреть на конкретную задачу, преспективнее всех выглядит Kafka, он быстро обрабатывает большие объемы данных, хранит постоянно все сообщения и позволяет их перечитывать.  

---

Подчеркну что оба ответа это скажет так мнение вне рамок конкретных ситуаций, тоесть для каждого проекта стоит отдельно проводить исследование и понимать какой конкретно API и брокер нам подойдут лучше всего.  