---
title: Тип ресурса Endpoint
description: Тип конечной точки
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3caf85f049c0b09caf5ae2ec3866ce9d24b2a1e8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601477"
---
# <a name="endpoint-resource-type"></a>Тип ресурса Endpoint

Пространство имен: microsoft.graph.callRecords

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
