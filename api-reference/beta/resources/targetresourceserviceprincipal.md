---
title: Тип ресурса targetResourceServicePrincipal
description: Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита. На основе targetResource ресурсов.
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839601"
---
# <a name="targetresourceserviceprincipal-resource-type"></a>Тип ресурса targetResourceServicePrincipal
Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита. На основе [targetResource](targetresource.md) ресурсов.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appId|String|Указывает уникальный идентификатор приложения. Указатель идентификатор приложения для приложения содержится код.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
