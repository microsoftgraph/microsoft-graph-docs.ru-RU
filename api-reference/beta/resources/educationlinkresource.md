---
title: Тип ресурса educationLinkResource
description: Подкласс educationResource. Этот ресурс является ссылкой и не имеют дополнительные данные, связанные с ним.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 09e7c7c5070d6f8f288dbf18d6fb9ce81b456092
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516961"
---
# <a name="educationlinkresource-resource-type"></a>Тип ресурса educationLinkResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс [educationResource](educationresource.md). Этот ресурс является ссылкой и не имеют дополнительные данные, связанные с ним.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ссылка|String|URL-адрес для ресурса.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationlinkresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
