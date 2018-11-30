---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
ms.openlocfilehash: 7669caa27be93786d381266f88b41ae456314bb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082585"
---
# <a name="windowsupdatetype-enum-type"></a>Тип перечисления windowsUpdateType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Какие устройства филиала будет получать обновления из
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|userDefined|0|Пользователь может задать.|
|all|1|Разделитель годовая канала (целевой). Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).|
|businessReadyOnly|2|Разделитель годовая канала. Устройства получает обновления компонента точками годовая канала.|
|windowsInsiderBuildFast|3|Построение изнутри Windows - Fast|
|windowsInsiderBuildSlow|4|Построение изнутри Windows - снижение производительности|
|windowsInsiderBuildRelease|5|Построение выпуска Windows изнутри|





