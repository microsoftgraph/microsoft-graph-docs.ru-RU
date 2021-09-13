---
title: тип ресурса plannerChecklistItem
description: Ресурс **plannerChecklistItem** представляет элемент в списке задач. Контрольный список задачи представлен объектом checklistItems.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a8ba68b0b9e9bb3bf6979ad9eb3d498fe55b80ee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113548"
---
# <a name="plannerchecklistitem-resource-type"></a>тип ресурса plannerChecklistItem

Пространство имен: microsoft.graph


Ресурс **plannerChecklistItem** представляет элемент в списке задач. Контрольный список задачи представлен [объектом checklistItems.](plannerchecklistitems.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isChecked|Логический|Значение, `true` если элемент проверяется и в `false` противном случае.|
|lastModifiedBy|[identitySet](identityset.md)| Только для чтения. Пользовательский ID, с помощью которого он был изменен в последний раз.|
|lastModifiedDateTime|DateTimeOffset|Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|orderHint|String|Используется для набора относительного порядка элементов в списке. Формат определяется как описанный [здесь](planner-order-hint-format.md).|
|title|String|Название элемента контрольного списка|

## <a name="json-representation"></a>Представление JSON
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

