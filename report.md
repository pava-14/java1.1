# Отчёт о тестировании KeyValidator

## Краткое описание

27.04.2020 - 28.04.2020 было проведено тестирование документации, дымовое тестирование приложения KeyValidator.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:
* https://github.com/pava-14/java1.1/issues/1
* https://github.com/pava-14/java1.1/issues/2
* https://github.com/pava-14/java1.1/issues/3
* https://github.com/pava-14/java1.1/issues/4

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* Инструкция по установке OpenJDK 11:
    https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md
* Руководство использования KeyValidator:
    https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md


В качестве тестовых данных, использовались данные из Руководства использования KeyValidator:
* Список валидных ключей:
1. 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998
2. 80b427f8-92cd-3aae-ba04-3927fbe17c6
3. b295bc63-9f03-3b4b-af80-969b39f8c262
4. 387eedc6-12e9-3b32-9881-63b6b5e85317
5. c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180

Ожидаемый результат на валидные ключи:
OK - в выводе KeyValidator. 

* Список невалидных ключей:
1. 18252235-78e0-44a5-8720-556f0c7da17a
2. e66075b6-ddad-445e-baf6-161b3289522b
3. b6d53250-f07e-4352-a293-6102ddf7f1ca
4. c2bc778a-1cb9-46c6-b435-0489649d2a42
5. 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1

Ожидаемый результат на невалидные ключи:
FAIL - в выводе KeyValidator.

Тестирование производилось в следующем окружении:
* ОС Windows 10 version 1909 64-bit
* openjdk version "11.0.7" 2020-04-14
* OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.7+10)
* OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.7+10, mixed mode)
