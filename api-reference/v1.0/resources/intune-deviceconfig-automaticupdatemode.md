---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
ms.openlocfilehash: c98927e1c1f66e3bf10fa07496aa54ac91bad20b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024853"
---
# <a name="automaticupdatemode-enum-type"></a>Тип перечисления automaticUpdateMode

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



