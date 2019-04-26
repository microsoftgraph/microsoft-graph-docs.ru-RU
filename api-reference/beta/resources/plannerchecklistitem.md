---
title: Тип ресурса Планнерчекклиститем
description: Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом Чекклиститемс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: deb168fa123c893d0d3793b0e67f65b6da2819b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344503"
---
# <a name="plannerchecklistitem-resource-type"></a>Тип ресурса Планнерчекклиститем

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен [объектом чекклиститемс](plannerchecklistitems.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|с возвратом|Логический|Значение, `true` если элемент отмечен флажком и `false` в противном случае.|
|lastModifiedBy|[identitySet](identityset.md)| Только для чтения. Идентификатор пользователя, на который последний раз изменился.|
|lastModifiedDateTime|DateTimeOffset|Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
