---
title: Тип ресурса Таржетполициендпоинтс
description: Представляет платформы, предназначенные для уведомлений пользователей.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: daac7a8424666d3974512c1cc1b17ec8e6878d7e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985666"
---
# <a name="targetpolicyendpoints-resource-type"></a>Тип ресурса Таржетполициендпоинтс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет платформы, которые могут быть предназначены для получения уведомлений, отправляемых пользователю.  К ним относятся Windows, iOS, Android и веб-сайт. 


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|платформтипес|Коллекция String|Используется для фильтрации распространения уведомлений на определенную платформу или платформы. Допустимые значения `Windows` : `iOS` , `Android` и `WebPush` . По умолчанию все типы конечных точек Push (Windows, iOS, Android и Push) включены. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetPolicyEndpoints",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetPolicyEndpoints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

