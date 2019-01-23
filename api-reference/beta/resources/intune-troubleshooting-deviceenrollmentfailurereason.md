---
title: Тип перечисления deviceEnrollmentFailureReason
description: Категории верхнего уровня failure для регистрации.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbfe7193c72f1ff1a03a7e7bb4da57d0a032e530
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396212"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>Тип перечисления deviceEnrollmentFailureReason

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




