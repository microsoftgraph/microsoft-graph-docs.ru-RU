---
title: Тип ресурса educationPowerPointResource
description: 'Подкласс educationResource. Это ресурсов PowerPoint. Необходимо отправить файл PowerPoint в каталоге **fileResource** , связанный с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512201"
---
# <a name="educationpowerpointresource-resource-type"></a>Тип ресурса educationPowerPointResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс [educationResource](educationresource.md). Это ресурсов PowerPoint. В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл PowerPoint.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|FileURL|String|Расположение файла на диске.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerpointresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
