---
title: Тип ресурса extension
description: Абстрактный тип для поддержки открытого типа openTypeExtension в OData 4-й версии.
localization_priority: Normal
ms.openlocfilehash: b261ceeff4639b8a602edbb411b34ab19d46ea8e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512747"
---
# <a name="extension-resource-type"></a>Тип ресурса extension

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип для поддержки открытого типа [openTypeExtension](opentypeextension.md) в OData 4-й версии.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|

## <a name="relationships"></a>Отношения
Нет


## <a name="methods"></a>Методы

Фактически поддерживаемые методы указаны в описании производного типа [openTypeExtension](opentypeextension.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
