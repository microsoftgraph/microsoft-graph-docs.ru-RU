---
title: Тип ресурса plannerChecklistItem
description: Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом пункты памятки.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fef935dfc2683e04b0ccec9ab5a7885927f8a13c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962984"
---
# <a name="plannerchecklistitem-resource-type"></a>Тип ресурса plannerChecklistItem

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список задачи представлен [объектом checklistItems](plannerchecklistitems.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isChecked|Логический|Значение — `true`, если элемент проверен, в противном случае — `false`.|
|lastModifiedBy|[identitySet](identityset.md)| Только для чтения. Идентификатор автора последних изменений.|
|lastModifiedDateTime|DateTimeOffset|Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|orderHint|Строка|Используется для указания относительного порядка элементов в списке. Используемый формат описан [здесь](planner-order-hint-format.md).|
|title|Строка|Название элемента списка|

## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
