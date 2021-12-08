---
title: тип ресурса clientUserAgent
description: Тип clientUserAgent
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aec85e917c8029d80da64eea9d9dc45f0c5070e5
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345905"
---
# <a name="clientuseragent-resource-type"></a>тип ресурса clientUserAgent

Пространство имен: microsoft.graph.callRecords

Представляет клиентского агента пользователя конечной точки в вызове. Наследуется от [типа userAgent.](callrecords-useragent.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого этой конечной точкой.|
|headerValue|Строка|Значение заглавной точки пользователя-агента, сообщаемого этой конечной точкой.|
|платформа|microsoft.graph.callRecords.clientPlatform|Определяет платформу, используемую этой конечной точкой. Возможные значения: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|microsoft.graph.callRecords.productFamily|Определяет семейство программного обеспечения приложения, используемого этой конечной точкой. Возможные значения: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`, `azureCommunicationServices`. Обратите внимание, что вы должны использовать загон запроса, чтобы получить следующее значение `Prefer: include-unknown-enum-members` (ы) в этом [развиваемом переуме:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `azureCommunicationServices` .|

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
