# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

15:00 - 16:00 было проведено системное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1 час.

В результате тестирования выявлены следующие дефекты:
* https://github.com/d-AMigo/Credit-Card-Number-Validator/issues/1
* https://github.com/d-AMigo/Credit-Card-Number-Validator/issues/2

## Описание процесса тестирования

В процессе тестирования использовался следующий артефакт:
* Check-list for Credit Card Number Validator

В качестве тестовых данных использовались данные freeformatter.com (https://www.freeformatter.com/credit-card-number-generator-validator.html) и собственные данные:
* Валидный номер карты 4969289030458657 возвращает Result is OK
* Валидный номер карты 5273419417109965 возвращает Result is OK
* Валидный номер карты 4929146341055628662 возвращает Result is OK
* Валидный номер карты 6011993192469023274 возвращает Result is OK
* Пустое значение String number возвращает Result is FAIL
* Пробел в значении String number возвращает Result is FAIL
* 0 в значении String number возвращает Result is FAIL
* -1 в значении String number возвращает Result is FAIL
* 0000000000000000 в значении String number возвращает Result is FAIL
* Credit Card Number в значении String number возвращает Result is FAIL


Тестирование производилось в следующем окружении:
* Windows 7, x64
* openjdk version "11.0.8" 2020-07-14
* git version 2.28.0.windows.1
* IntelliJ IDEA 2020.2.1 (Community Edition)
Build #IC-202.6948.69, built on August 25, 2020
