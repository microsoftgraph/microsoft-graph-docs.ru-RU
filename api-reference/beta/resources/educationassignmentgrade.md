---
title: Тип ресурса Едукатионассигнментграде
description: " Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5ca13ba057ef000a468d910d49288d9ae8e0c962
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543023"
---
# <a name="educationassignmentgrade-resource-type"></a>Тип ресурса Едукатионассигнментграде

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект **Grade** при отправке. Это абстрактный тип, экземпляры которого никогда не будут создаваться; Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого типа ресурсов. Кроме того, этот объект отслеживает круг пользователей, выполняющих ступенчатое выполнение. Используется в свойстве **отсылки. Grade** .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Градедби|[identitySet](identityset.md)| Пользователь, который выполнил ступенчатое. |
|Градеддатетиме|DateTimeOffset| Момент времени, когда уровень был применен к этому объекту отправки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
