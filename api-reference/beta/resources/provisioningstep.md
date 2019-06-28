---
title: Тип ресурса Провисионингстеп
description: 'Описывает действия, предпринимаемые для выполнения действия. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1658114615c4532f0a7f9b9f5ad3c3a25deff81b
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349437"
---
# <a name="provisioningstep-resource-type"></a>Тип ресурса Провисионингстеп

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает действия, предпринимаемые для выполнения действия.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Сводка действий, произошедших на этапе.|
|details|[Детаилсинфо](detailsinfo.md)|Сведения о том, что произошло на этапе.|
|name|String|Имя этапа.|
|Провисионингстептипе|String| Тип этапа. Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|String| Состояние этапа. Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
