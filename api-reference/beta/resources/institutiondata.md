---
title: Тип ресурса Институтиондата
description: Тип ресурса Институтиондата
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5724f56a5e68c059126eaac910d34999dcded632
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939455"
---
# <a name="institutiondata-resource-type"></a>Тип ресурса Институтиондата

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет дополнительные сведения о выпуске, выпускнике, степени выпуске или других образовательных действиях, выполняемых пользователем и используемом в ресурсе [едукатионалактивити](educationalActivity.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип                                 | Описание                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|description   |String                                |Краткое описание учебного заведения, в котором пользователь изучается. |
|displayName   |Строка                                |Имя учреждения, в котором пользователь изучается.              |
|location      |[physicalAddress](physicaladdress.md) |Адрес или расположение института.                     |
|webUrl        |String                                |Ссылка на домашнюю страницу "учреждение" или "Отдел".           |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->