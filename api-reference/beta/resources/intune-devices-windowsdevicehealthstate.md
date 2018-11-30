---
title: Тип перечисления windowsDeviceHealthState
description: Состояние защиты компьютера конечной точки
ms.openlocfilehash: 601531dd71ee0d44e9f5ebc89eb018ba5e0f2675
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074676"
---
# <a name="windowsdevicehealthstate-enum-type"></a>Тип перечисления windowsDeviceHealthState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние защиты компьютера конечной точки
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|clean|0|Компьютер чистой и никаких действий не требуется|
|fullScanPending|1|Компьютер находится в состоянии полную проверку ожидания|
|rebootPending|2|Компьютер находится в состоянии перезагрузки ожидания|
|manualStepsPending|4|Компьютер находится в состоянии ручные операции ожидания|
|offlineScanPending|8|Компьютер находится в состоянии автономной проверки ожидания|
|critical|16|Компьютер находится в состоянии критическая ошибка|





