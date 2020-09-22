---
title: Тип ресурса Шифтактивити
description: Представляет действие в смене.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 564e00b14bbfe9e5a0cde8a09897d24ea81e0a96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970693"
---
# <a name="shiftactivity-resource-type"></a>Тип ресурса Шифтактивити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие в [смене](shift.md).

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| Предопл               | `bool`                  | Указывает, `microsoft.graph.user` следует ли платить за действие в течение этого периода `shift` . Обязательно.    |
| startDateTime               | `DateTimeOffset`                  | Дата и время начала для ресурса `shiftActivity`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". Обязательный элемент. |
| endDateTime               | `DateTimeOffset`                  | Дата и время окончания для ресурса `shiftActivity`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". Обязательный элемент.    |
| code               | `string`                  | Определенный пользователем код для `shiftActivity` . Обязательный.    |
| displayName               | `string`                  | Имя ресурса `shiftActivity`. Обязательный элемент.    |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

