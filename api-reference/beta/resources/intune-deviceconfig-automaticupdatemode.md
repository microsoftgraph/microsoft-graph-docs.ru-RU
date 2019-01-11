---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 08389dca4379b6fc0222068545ebb9bed250ba94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863415"
---
# <a name="automaticupdatemode-enum-type"></a>Тип перечисления automaticUpdateMode

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для режима автоматического обновления.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|notifyDownload|1|Уведомите при загрузке.|
|autoInstallAtMaintenanceTime|2|Автоматическая установка с во время обслуживания.|
|autoInstallAndRebootAtMaintenanceTime|3|Установить и перезагрузите во время обслуживания.|
|autoInstallAndRebootAtScheduledTime|4|Установить и перезагрузите компьютер в запланированное время.|
|autoInstallAndRebootWithoutEndUserControl|5|Установить и перезапустите без управления конечных пользователей|





