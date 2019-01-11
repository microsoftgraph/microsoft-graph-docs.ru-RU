---
title: Тип перечисления deviceEnrollmentFailureReason
description: Категории верхнего уровня failure для регистрации.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd7ba949c95d507d956dd7f315b3c19e0759c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885528"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>Тип перечисления deviceEnrollmentFailureReason

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Категории верхнего уровня failure для регистрации.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию причина сбоя не известен.|
|проверка подлинности|1|Ошибка проверки подлинности|
|авторизация|2|Звонок был прошедшим проверку подлинности, но не разрешена для регистрации.|
|accountValidation|3|Не удается проверить учетную запись для регистрации. (Учетная запись заблокирована, регистрации не включена)|
|userValidation|4|Пользователь не может быть проверен. (Пользователь не существует, отсутствует лицензия)|
|deviceNotSupported|5|Устройство не поддерживается для мобильных устройств management.|
|inMaintenance|6|Учетная запись является в режим обслуживания.|
|badRequest|7|Клиент отправил запрос, который не является поняты/поддерживается службой.|
|featureNotSupported|8|Компоненты, используемые в этом регистрации не поддерживается для этой учетной записи.|
|enrollmentRestrictionsEnforced|9|Ограничения для регистрации настроены администратором заблокированные этой регистрации.|
|clientDisconnected|10|Истекло время ожидания клиента или регистрации был прерван пользователем enduser.|
|userAbandonment|11|Регистрация отменена с enduser. (Enduser работы адаптация новых сотрудников, но не удалось завершить своевременно)|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
