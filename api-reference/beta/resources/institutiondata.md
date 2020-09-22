---
title: Тип ресурса Институтиондата
description: Тип ресурса Институтиондата
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a528bf5bc8800b10deed2c45d84613b5ab4bd6b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986075"
---
# <a name="institutiondata-resource-type"></a>Тип ресурса Институтиондата

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет дополнительные сведения о выпуске, выпускнике, степени выпуске или других образовательных действиях, выполняемых пользователем и используемом в ресурсе [едукатионалактивити](educationalActivity.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип                                 | Описание                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|description   |String                                |Краткое описание учебного заведения, в котором пользователь изучается. |
|displayName   |String                                |Имя учреждения, в котором пользователь изучается.              |
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

