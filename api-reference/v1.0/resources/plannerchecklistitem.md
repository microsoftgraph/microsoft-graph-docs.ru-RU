---
title: Тип ресурса Планнерчекклиститем
description: Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом Чекклиститемс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b0f7a33393ca69c863eecb91738ee7394218f5b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534007"
---
# <a name="plannerchecklistitem-resource-type"></a>Тип ресурса Планнерчекклиститем

Пространство имен: microsoft.graph


Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен [объектом чекклиститемс](plannerchecklistitems.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|с возвратом|Boolean|Значение, `true` если элемент отмечен флажком и `false` в противном случае.|
|lastModifiedBy|[identitySet](identityset.md)| Только для чтения. Идентификатор пользователя, на который последний раз изменился.|
|lastModifiedDateTime|DateTimeOffset|Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|orderHint|String|Используется для задания относительного порядка элементов в контрольном списке. Формат определяется, как описано [ниже](planner-order-hint-format.md).|
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
