---
title: Тип ресурса Едукатионресаурце
description: Суперкласс для всех объектов ресурсов в системе. Ресурс связан с наЗначением **** и/или отправкой, представляющим обучающий объект, который ****
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 87b19f849e24f1780a1d13c7aa1b3eb83543fdec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542879"
---
# <a name="educationresource-resource-type"></a>Тип ресурса Едукатионресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Суперкласс для всех объектов ресурсов в системе. Ресурс связан с наЗначением **** и/или отправкой, представляющим обучающий объект, который передается или передается. **** Невозможно напрямую создать экземпляр ресурса; необходимо создать подкласс, который будет представлять тип используемого ресурса.

В этом ресурсе хранятся общие свойства для всех типов ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Кто создал ресурс.|
|createdDateTime|Момент создания ресурса.  DateTimeOffset|Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayName|String|Отображаемое имя ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Кто последний пользователь изменил ресурс.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
