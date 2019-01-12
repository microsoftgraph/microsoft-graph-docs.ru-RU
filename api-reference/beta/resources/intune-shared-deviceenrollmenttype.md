---
title: Тип перечисления deviceEnrollmentType
description: Возможные способы добавления мобильного устройства для управления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bffe0e592240cbeee22a63dac8c339a0d3b3ff3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946842"
---
# <a name="deviceenrollmenttype-enum-type"></a>Тип перечисления deviceEnrollmentType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные способы добавления мобильного устройства для управления.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Тип регистрации значения по умолчанию не собираются.|
|userEnrollment|1|Регистрация управляемых пользователя по каналу BYOD.|
|deviceEnrollmentManager|2|Регистрация пользователя с учетной записью диспетчера устройств заявок через Интернет.|
|appleBulkWithUser|3|Регистрация массового Apple с запрос пользователя. (DEP конфигуратора Apple)|
|appleBulkWithoutUser|4|Apple массового заявок через Интернет без запроса пользователя. (DEP конфигуратора Apple мобильных Config)|
|windowsAzureADJoin|5|Присоединение к Windows Azure AD 10.|
|windowsBulkUserless|6|Массовое 10 Windows подачи заявок через ICD с сертификатом.|
|windowsAutoEnrollment|7|Windows 10 автоматической подачи заявок. (Добавление учетной записи работы)|
|windowsBulkAzureDomainJoin|8|Windows 10 в пакетном режиме присоединиться к Azure AD.|
|windowsCoManagement|9|10 совместного управления Windows активировать по автопилот или групповой политики.|





