---
title: Тип перечисления roleAssignmentScopeType
description: Указывает тип области для назначения ролей.
author: tfitzmac
ms.openlocfilehash: 0a3286b3b7bc583323204ca39ff85e01869ddbe7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343129"
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





