---
title: Тип ресурса Статусбасе
description: Описывает состояние сводного события подготовки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: de35e89b674130bb1f2896b299ba5f4efe3af099
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349453"
---
# <a name="statusbase-resource-type"></a>Тип ресурса Статусбасе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние сводного события подготовки. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String| Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusBase",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
