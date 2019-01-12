---
title: Тип перечисления windowsDeviceHealthState
description: Состояние защиты компьютера конечной точки
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923945"
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





