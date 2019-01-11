---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 51ed838b6abaaf36a69230b566c01b8d496c2a70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872074"
---
# <a name="defendercloudblockleveltype-enum-type"></a>Тип перечисления defenderCloudBlockLevelType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения уровня блока облако
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение по умолчанию использует блокировки антивирусной программы Защитник Windows по умолчанию на уровне и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимые файлов|
|Высокая|1|High применяется повышенный уровень обнаружения.|
|highPlus|2|Высокая + использует высокий уровень и предоставляет средства защиты сложения|
|zeroTolerance|3|Ноль отказоустойчивости блокирует все неизвестные исполняемых файлов|





