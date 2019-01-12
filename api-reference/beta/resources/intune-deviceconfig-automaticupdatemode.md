---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20aa217838848af6d85c023fd6587afe3427e82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913270"
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





