---
title: Тип перечисления roleAssignmentScopeType
description: Указывает тип области для назначения ролей.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b72e74bdb401f556214470b4c0aeda651339e332
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916084"
---
# <a name="roleassignmentscopetype-enum-type"></a>Тип перечисления roleAssignmentScopeType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Указывает тип области для назначения ролей.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|resourceScope|0|Разрешить назначения для указанного ResourceScopes.|
|allDevices|1|Разрешить назначений на все устройства Intune.|
|allLicensedUsers|2|Разрешить назначения для всех пользователей с корпоративным лицензированием Intune.|
|allDevicesAndLicensedUsers|3|Разрешить назначения для всех устройств Intune и лицензированных пользователей.|





