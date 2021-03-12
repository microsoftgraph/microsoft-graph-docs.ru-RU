---
title: тип ресурса shiftActivity
description: Представляет действие в сдвиге.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 30552f0a5c856d0144fd231cda6b9e1aa825d97f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721798"
---
# <a name="shiftactivity-resource-type"></a>тип ресурса shiftActivity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие в [сдвиге.](shift.md)

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| isPaid               | `bool`                  | Указывает, следует ли платить за действия во `microsoft.graph.user` время их `shift` . Обязательный.    |
| startDateTime               | `DateTimeOffset`                  | Дата и время начала для ресурса `shiftActivity`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Обязательный элемент. |
| endDateTime               | `DateTimeOffset`                  | Дата и время окончания для ресурса `shiftActivity`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Обязательный.    |
| code               | `string`                  | Код, определенный клиентом `shiftActivity` для . Обязательный.    |
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

