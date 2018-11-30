---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
ms.openlocfilehash: 70e43e9659e7dd7be1d3c0a190e21d80d7b8dc41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080319"
---
# <a name="defendercloudblockleveltype-enum-type"></a>Тип перечисления defenderCloudBlockLevelType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения уровня блока облако
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|notConfigured|0|Значение по умолчанию использует блокировки антивирусной программы Защитник Windows по умолчанию на уровне и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимые файлов|
|Высокая|1|High применяется повышенный уровень обнаружения.|
|highPlus|2|Высокая + использует высокий уровень и предоставляет средства защиты сложения|
|zeroTolerance|3|Ноль отказоустойчивости блокирует все неизвестные исполняемых файлов|





