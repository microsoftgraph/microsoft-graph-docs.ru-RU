---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 13f8828478eb063eaa25d8561d5a254c86f4b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924722"
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





