---
title: Тип ресурса Клиентусеражент
description: Тип Клиентусеражент
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d2024e4263da379ab42c2878bc18e0a2d3ec27ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069449"
---
# <a name="clientuseragent-resource-type"></a>Тип ресурса Клиентусеражент

Пространство имен: microsoft.graph.callRecords

Представляет агент пользователя клиента конечной точки в вызове. Наследуется от типа [UserAgent](callrecords-useragent.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого конечной точкой.|
|headerValue|Строка|Значение заголовка User — Agent, указанное конечной точкой.|
|платформа|Microsoft. Graph. Каллрекордс. Клиентплатформ|Определяет платформу, используемую этой конечной точкой. Возможные значения: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|продуктфамили|Microsoft. Graph. Каллрекордс. Продуктфамили|Определяет семейство программного обеспечения приложений, используемое этой конечной точкой. Возможные значения: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "platform": "String",
  "productFamily": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "clientUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
