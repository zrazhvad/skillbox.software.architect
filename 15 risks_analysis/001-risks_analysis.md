# Анализ рисков, компромисов

## Программисты

Поскольку решено не нанимать в штат мобильных разработчиков, разработку будут вести текущие frontend разработчики. В виду отсутствия необходимого опыта в нужном количестве есть вероятность задержки сдачи проекта мобильного приложения. Следует обратить внимание на требования по носимой электронике и трекингу тренировок мобильным устройством. Возможно имеет смысл отправить разработчиков на курсы мобильной разработки.

## Debezium

Требуются испытания работы этого программного обеспечения на платформе VK Cloud и обсуждение возможности реализации необходимых настроек Postgres на с провайдером. Возможна задержка по времени в случае если выяснится что необходимый функционал при живых испытаниях работает не так как ожидалось и требует исправления на стороне провайдера.

## Денормализованная база данных для запросов

Нужно учитывать что данные в документориентированной базе данных будут условно - консистентные, так как требуется синхронизация из консистентного хранилища.

## Горизонтальное масштабирование

Нужно учитывать что в момент времени будет развернуто N инстансов каждого сервиса, соответственно требуется обязательное тестирование системы с учетом такого масштабирования. Все очереди должны работать в соответствии с заданными целями (например, если предполагается параллельная обработка множества атомарных операций, требуется убедиться что одно и то же сообщение не обработано двумя и более экземплярами сервиса)

## Очереди

Брокеры очередей могут стать недоступны. Требуется реализация системы с мониторингом и уведомлениями в случае если брокер вышел из строя.

## Санкции

Требуется учитывать возможное закрытие того или иного ПО в Российской Федерации и по возможности использовать ПО которое с наименьшей вероятностью уйдет из страны или же перестанет поддерживаться. 