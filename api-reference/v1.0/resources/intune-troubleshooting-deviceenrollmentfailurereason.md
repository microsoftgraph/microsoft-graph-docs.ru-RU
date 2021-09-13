---
title: тип enum deviceEnrollmentFailureReason
description: Категории отказов верхнего уровня для регистрации.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 39c422f50c1ff68cabdc12eed92855167347bbab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021549"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>тип enum deviceEnrollmentFailureReason

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Категории отказов верхнего уровня для регистрации.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию, причина сбоя неизвестна.|
|проверка подлинности|1|Сбой проверки подлинности|
|авторизация|2|Вызов был аутентификацией, но не разрешен для регистрации.|
|accountValidation|3|Не удалось проверить учетную запись для регистрации. (Учетная запись заблокирована, регистрация не включена)|
|userValidation|4 |Пользователь не может быть проверен. (Пользователь не существует, отсутствует лицензия)|
|deviceNotSupported|5 |Устройство не поддерживается для управления мобильными устройствами.|
|inMaintenance|6 |Учетная запись находится в обслуживании.|
|badRequest|7 |Клиент отправил запрос, который не понят или поддерживается службой.|
|featureNotSupported|8 |Функция(ы), используемая этой учетной записью, не поддерживается.|
|enrollmentRestrictionsEnforced|9 |Ограничения регистрации, настроенные администратором, заблокировали эту регистрацию.|
|clientDisconnected|10 |Клиент, отовремя отсев или регистрация, был прерван enduser.|
|userAbandonment|11|Регистрация была отменена enduser. (Enduser начал работать на борту, но не удалось выполнить его своевременно)|




