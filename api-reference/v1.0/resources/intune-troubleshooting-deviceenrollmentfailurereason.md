---
title: тип enum deviceEnrollmentFailureReason
description: Категории отказов верхнего уровня для регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f47c4903c17d8c99408449d32b83a38a7389204
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266634"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>тип enum deviceEnrollmentFailureReason

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Категории отказов верхнего уровня для регистрации.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию, причина сбоя неизвестна.|
|проверка подлинности|1 |Сбой проверки подлинности|
|авторизация|2|Вызов был аутентификацией, но не разрешен для регистрации.|
|accountValidation|3 |Не удалось проверить учетную запись для регистрации. (Учетная запись заблокирована, регистрация не включена)|
|userValidation|4 |Пользователь не может быть проверен. (Пользователь не существует, отсутствует лицензия)|
|deviceNotSupported|5 |Устройство не поддерживается для управления мобильными устройствами.|
|inMaintenance|6 |Учетная запись находится в обслуживании.|
|badRequest|7 |Клиент отправил запрос, который не понят или поддерживается службой.|
|featureNotSupported|8 |Функция(ы), используемая этой учетной записью, не поддерживается.|
|enrollmentRestrictionsEnforced|9 |Ограничения регистрации, настроенные администратором, заблокировали эту регистрацию.|
|clientDisconnected|10 |Клиент, отовремя отсев или регистрация, был прерван enduser.|
|userAbandonment|11 |Регистрация была отменена enduser. (Enduser начал работать на борту, но не удалось выполнить его своевременно)|




