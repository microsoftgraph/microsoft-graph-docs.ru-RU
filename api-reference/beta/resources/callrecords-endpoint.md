---
title: Тип ресурса Endpoint
description: Тип конечной точки
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f17aa21de65fef33b0c7e4a94151eab4f49583ac
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394860"
---
# <a name="endpoint-resource-type"></a>Тип ресурса Endpoint

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет конечную точку в вызове. Конечной точкой может быть устройство пользователя, собрание, приложение/Bot и т. д. Типы [партиЦипантендпоинт](callrecords-participantendpoint.md) и [сервицеендпоинт](callrecords-serviceendpoint.md) наследуются от этого типа.

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
  "@odata.type": "microsoft.graph.callRecords.endpoint",
  "baseType": null
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
  "description": "endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->