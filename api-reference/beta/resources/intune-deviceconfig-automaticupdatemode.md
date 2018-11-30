---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080587"
---
# <a name="automaticupdatemode-enum-type"></a>Тип перечисления automaticUpdateMode

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для режима автоматического обновления.
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|notifyDownload|1|Уведомите при загрузке.|
|autoInstallAtMaintenanceTime|2|Автоматическая установка с во время обслуживания.|
|autoInstallAndRebootAtMaintenanceTime|3|Установить и перезагрузите во время обслуживания.|
|autoInstallAndRebootAtScheduledTime|4|Установить и перезагрузите компьютер в запланированное время.|
|autoInstallAndRebootWithoutEndUserControl|5|Установить и перезапустите без управления конечных пользователей|





