<div align="center">
  
University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FTMI](https://ftmi.itmo.ru/)

Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) 

Year: 2024

Group: U4225

Author: Popova Anna Andreevna

Lab: Lab2

Date of create: 25.10.2024

Date of finished: 25.10.2024

1. Использовала Google Cloud Console для создания нового сервиса Cloud Run на основе дефолтного образа Hello. После успешного создания был предоставлен URL Cloud Run.
<img width="1345" alt="image" src="https://github.com/user-attachments/assets/63e86151-80f2-4a84-a8ea-15410cfac697">
2. Перешла по ссылке предоставленной Cloud Run и протестировала сервис. Тестирование показало, что сервис отвечает на запросы корректно, с минимальной задержкой.
<img width="854" alt="image" src="https://github.com/user-attachments/assets/f8294fa5-43f7-4c67-8ed3-6e096abcd58c">
3. Перешла в раздел Logs через интерфейс Cloud Run. Проанализировала логи, которые включали информацию о каждом запросе, времени отклика и состоянии выполнения.
Логи не содержали ошибок, что подтверждает корректную работу сервиса.
<img width="1309" alt="image" src="https://github.com/user-attachments/assets/144fafdb-d0be-49ec-9c67-4f2b00146432">
4.Перешла в раздел Metrics в консоли Cloud Run.Обратила внимание на такие показатели, как:
Latency (задержка) — низкие значения, что говорит о быстрой обработке запросов.
CPU Usage и Memory Usage — использовались в пределах заданных лимитов.
Метрики позволили оценить производительность и стабильность работы сервиса при тестовых запросах.
<img width="1708" alt="image" src="https://github.com/user-attachments/assets/ce74b6d2-6c2b-4bd8-8a81-14ce97ec96d6">
5. Изменила конфигурацию Cloud Run, установив порт 8090:
В настройках сервиса добавила переменную окружения PORT=8090.
Перезапустила сервис с новой версией.
Сервис успешно заработал на новом порте. Важно отметить, что в Cloud Run автоматически осуществляется маршрутизация, поэтому URL остался прежним, а изменения коснулись только внутренней настройки.
Проверила работу сервиса после изменения порта, чтобы убедиться в корректной обработке запросов.
<img width="1684" alt="image" src="https://github.com/user-attachments/assets/4a868bf6-a762-4703-ac4e-a6d9b61f1278">
6. В разделе Revisions распределила трафик между старой и новой версиями (50% на версию с портом 8080 и 50% на версию с портом 8090). Выполнила тестовые запросы для проверки распределения трафика между версиями. В логах отразилась работа обеих версий, что подтвердило корректное распределение трафика. Сравнение метрик показало, что обе версии обрабатывают запросы одинаково, без значительных различий в производительности.


</div>
