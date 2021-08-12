---
title: тип ресурса clientUserAgent
description: Тип clientUserAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6c1150cf60b3b042358ff1a854944b14722e2a9717daaed064d9d63392e475aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212215"
---
# <a name="clientuseragent-resource-type"></a>тип ресурса clientUserAgent

Пространство имен: microsoft.graph.callRecords

Представляет клиентского агента пользователя конечной точки в вызове. Наследуется от [типа userAgent.](callrecords-useragent.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого этой конечной точкой.|
|headerValue|String|Значение заглавной точки пользователя-агента, сообщаемого этой конечной точкой.|
|платформа|microsoft.graph.callRecords.clientPlatform|Определяет платформу, используемую этой конечной точкой. Возможные значения: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|microsoft.graph.callRecords.productFamily|Определяет семейство программного обеспечения приложения, используемого этой конечной точкой. Возможные значения: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.|

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
