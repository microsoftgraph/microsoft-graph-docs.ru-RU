---
title: provisioningStatusInfo resource type
description: Описывает состояние события сводки по подготовкам.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7ab2a67662f6e03fd7f967757a7de7ec92480826
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682070"
---
# <a name="provisioningstatusinfo-resource-type"></a>provisioningStatusInfo resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние события сводки по подготовкам. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String| Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.|
|errorInfo|[provisioningErrorInfo](provisioningerrorinfo.md)| Если состояние не успешно или пропущенные сведения об ошибке содержатся в этом.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
  "baseType": null
}-->

```json
{
  "status": "String",
  "errorinfo": {"@odata.type": "microsoft.graph.provisioningErrorInfo"},}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStatusInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


