---
title: Тип ресурса Шифтитем
description: Шифтитем представляет версию смены.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd5b3d224e60fc3f21b4d484952c7a2643b02407
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343040"
---
# <a name="shiftitem-resource-type"></a>Тип ресурса Шифтитем

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет версию [смены](shift.md).

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | Примечания для `shiftItem`.      |
| displayName               | string                  | Имя файла `shiftItem`. |
| startDateTime               | DateTimeOffset                  | Дата и время начала для `shiftItem`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". Обязательный. |
| endDateTime               | DateTimeOffset                 | Дата и время окончания для `shiftItem`. Обязательный. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
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
