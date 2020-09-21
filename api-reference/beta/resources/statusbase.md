---
title: Тип ресурса Статусбасе
description: Описывает состояние сводного события подготовки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ee205db24cf8591725ca7d9fc3c4a0fe8c72489e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067106"
---
# <a name="statusbase-resource-type"></a>Тип ресурса Статусбасе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние сводного события подготовки. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String| Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление в формате JSON

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


