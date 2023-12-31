# Сценарии использования приложения

## Регистрация

1. Новый пользователь открывает страницу авторизации/аутентификации;
2. Выбирает кнопку "зарегистрировать нового пользователя", попадает на страницу регистрации нового пользователя;
3. Вводит регистрационные данные/анкету;
4. Вводит данные для yandex smartcaptcha;
5. Нажимает кнопку "Зарегистрировать", попадает на форму ввода кода подтверждения и предложение посетить свой почтовый клиент, так как код отправлен туда;
6. Вводит код, при успешном введенном коде попадает на страницу личного кабинета, при неуспешном - получает ошибку, и предложение ввести код повторно. После пяти неверных введенных кодов попытки блокируются на час.

## Авторизация/Аутентификация

1. Существующий пользователь открывает страницу авторизации/аутентификации;
2. Вводит свои регистрационные данные;
3. В случае если данные введены верно - пользователя переводит в личный кабинет;
4. В случае ошибки - пользователь получает сообщение об ошибке и предложение ввести данные снова.
5. После 5 неверных попыток, вход блокируется, на почту пользователя отправляется уведомление о том что кто то пытается войти в его аккаунт, на мобильное устройство приходит пуш уведомление с этой информацией.

## Поиск и регистрация в тематических группах

1. На вкладке "Группы" пользователь пользователь вводит в текстовое поле актуальную для поиска фразу;
2. В списке под полем поиска выводятся результаты;
3. Пользователь выбирает наиболее понравившуюся ему группу;
4. Пользователь нажимает кнопку "Вступить";
5. Если группа приватная - отправляется сообщение с запросом на вступление модератору группы;
6. Если группа открытая - пользователь становится участником группы и получает все новости и уведомления;

## Проведение тренировки с мобильным устройством

1. На вкладке "Тренировки" пользователь нажимает кнопку "Создать";
2. В открывшемся окне ему предлагается заполнить тип тренировки, выбрать носимое устройство а так же перечислить инвентарь который он использует;
3. Когда тренировка создана, она появится в списке тренировок на вкладке "Тренировки";
4. Далее, нажав кнопку "старт" пользователь начинает тренировку;
5. Данные по тренировке агрегируются в памяти мобильного устройства;
6. По завершению тренировки, пользователь нажимает кнопку "Стоп", система пытается синхронизировать эти данные с сервером раз в 30 секунд.
7. При успешной синхронизации пользователю предлагается поделиться результатами тренировки на своей "стене" или же в какой либо из групп, к которой у пользователя есть доступ; 
8. Так же по завершении тренировки пользователю предлагается принять участие в статистике, если он согласен, то его результаты будут приняты в сравнение с другими пользователями и будут доступны на общих дашбордах по данному типу тренировки;
9. Далее система предложит улучнить результаты путем покупки нового инвентаря в онлайн магазине, предложит товары на основании более успешных результатов других пользователей или же новинки или же товаров более высокого класса;

## Проведение соревнования

1. Пользователь получает новость о проведении соревнования;
2. Пользователь переходит на страницу новости и ознакамливается с условием соревнования;
3. Пользователь нажимает кнопку "подать заявку", и заполняет анкету соревнования;
4. Модератор ознакамливается со списком пользователей и в случае если пользователь подходит для этого соревнования - принимает заявку, пользователь получает ответ в личном сообщении;
5. За сутки до проведения мероприятия пользователь получает EMail и Push уведомления с инструкциями;
6. Соревнование проходит;
7. Модератор регистрирует данные о проведенном мероприятии;
8. Результаты соревнования появляются в новостной ленте;
9. Пользователь получает рекоммендации о покупке нового инвентаря на основе результатов его участия;

## Регистрация группы

1. Пользователь переходит на вкладку "Группы";
2. Пользователь нажимает кнопку "Зарегистрировать";
3. Пользователь заполняет форму и описание группы нажимает "подать заявку";
4. Группа проходит модерацию, при успешной модерации - группа опубликована;
5. Пользователь становится администратором группы, так же может сделать администратором кого то из своих друзей;