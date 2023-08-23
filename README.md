# SMEV
![alt text](https://github.com/disant9807/SMEV/blob/main/Schema.png?raw=true)

Микросервисное решение реализации адаптера СМЭВ. Представляет собой сервисы на java 8 JDK OpenLogic 8u372-b07, которая поддерживается в AstraLinux. Решение не реализовано до конца, часть сервисов представляет собой просто концепт.

# Сервис Gate Концепт (не реализован).
Основные задачи gate:
- Получить сообщение-запрос из СМЭВ, определить, кому предназначено данное сообщение и направить его в систему обработчик соответствующих запросов
- Получить ответ от системы-получателя, подписать его подписью ОИВ и направить его в СМЭВ.
- Получить запрос в СМЭВ извне, подписать его подписью ОИВ и отправить в СМЭВ.
- Получить сообщение-ответ на ранее отправленный запрос из СМЭВ и направить его в систему, которая отправляла запрос.
Концепт реализации обработки входящих запосов - [a link]([https://github.com/user/repo/blob/branch/other_file.md](https://github.com/disant9807/GateSmev/blob/master/server/src/main/java/ru/spandco/binstorage/server/sheduling/SmevRequestWatcher.java)https://github.com/disant9807/GateSmev/blob/master/server/src/main/java/ru/spandco/binstorage/server/sheduling/SmevRequestWatcher.java)
