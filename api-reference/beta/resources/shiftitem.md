---
title: Тип ресурса Шифтитем
description: Шифтитем представляет версию смены.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: df012df0ec563a29f15e40d3fefbcd1535dc5211
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008345"
---
# <a name="shiftitem-resource-type"></a>Тип ресурса Шифтитем

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет версию [смены](shift.md).

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | Примечания для `shiftItem`.      |
| displayName               | string                  | Имя файла `shiftItem`. |
| startDateTime               | DateTimeOffset                  | Дата и время начала для `shiftItem`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". Обязательно. |
| endDateTime               | DateTimeOffset                 | Дата и время окончания для `shiftItem`. Обязательно. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| theme | Счедулинтитисеме   |  Поддерживаемые цвета: белый; компонентов Интенсив цвет Розов желтый участка Даркблуе; Даркгрин; Даркпурпле; Даркпинк; Даркеллов. |
| activities    | Коллекция [шифтактивити](shiftactivity.md)   | Добавочная часть сдвига, в которой можно получить сведения о том, когда и где сотрудник наносится на свою смену. Например, назначение или запланированный перерыв или обед. Обязательное. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
