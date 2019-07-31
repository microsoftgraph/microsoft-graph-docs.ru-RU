---
title: Тип ресурса Едукатионассигнментграде
description: " Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4de74fc9cbdf505bd57cfad3ab8dbf5a12e4e58a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006474"
---
# <a name="educationassignmentgrade-resource-type"></a>Тип ресурса Едукатионассигнментграде

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект **Grade** при отправке. Это абстрактный тип, экземпляры которого никогда не будут создаваться; Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого типа ресурсов. Кроме того, этот объект отслеживает круг пользователей, выполняющих ступенчатое выполнение. Используется в свойстве **отсылки. Grade** .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Градедби|[identitySet](identityset.md)| Пользователь, который выполнил ступенчатое. |
|Градеддатетиме|DateTimeOffset| Момент времени, когда уровень был применен к этому объекту отправки. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
