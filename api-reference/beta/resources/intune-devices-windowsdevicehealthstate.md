---
title: Тип перечисления windowsDeviceHealthState
description: Состояние защиты компьютера конечной точки
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 91869502d0d61c25c6eb8dd67ba4e8e32d28fbb2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885927"
---
# <a name="windowsdevicehealthstate-enum-type"></a>Тип перечисления windowsDeviceHealthState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние защиты компьютера конечной точки
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|clean|0|Компьютер чистой и никаких действий не требуется|
|fullScanPending|1|Компьютер находится в состоянии полную проверку ожидания|
|rebootPending|2|Компьютер находится в состоянии перезагрузки ожидания|
|manualStepsPending|4|Компьютер находится в состоянии ручные операции ожидания|
|offlineScanPending|8|Компьютер находится в состоянии автономной проверки ожидания|
|critical|16|Компьютер находится в состоянии критическая ошибка|





