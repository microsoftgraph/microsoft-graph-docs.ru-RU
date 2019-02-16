---
title: Тип ресурса Посталаддресс
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7d168e4f53dbd182e4dbd93d0a5b6342daf3339d
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057413"
---
# <a name="postaladdress-resource-type"></a>Тип ресурса Посталаддресс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет почтовый адрес расположения.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Город.|
|countryOrRegion|String|Страна или регион. Это строковое значение в произвольном формате, например "США".|
|Исинферред|Boolean|Только для внутреннего использования.|
|postalCode|String|Почтовый индекс.|
|state|String|Штат.|
|street|String|Улица.|
|type|addressType|Тип адреса. `unknown`Возможные значения: `home`,, `business`,. `other`|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.postalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "isInferred": "boolean",
  "postalCode": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "postaladdress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/postaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
