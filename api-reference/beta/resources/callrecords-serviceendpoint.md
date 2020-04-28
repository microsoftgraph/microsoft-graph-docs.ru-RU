---
title: Тип ресурса Сервицеендпоинт
description: Тип Сервицеендпоинт
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9fe86f55615c4e7d58a219f15bd9e6792e5ae72b
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394806"
---
# <a name="serviceendpoint-resource-type"></a>Тип ресурса Сервицеендпоинт

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет конечную точку службы в вызове. Конечная точка представляет вызывающий медиа сервер или другой объект службы. Наследуется от типа [конечной точки](callrecords-endpoint.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|userAgent|[Microsoft. Graph. Каллрекордс. userAgent](callrecords-useragent.md)|Пользователь — агент, указанный этой конечной точкой.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->