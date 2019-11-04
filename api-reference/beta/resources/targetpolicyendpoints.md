---
title: Тип ресурса Таржетполициендпоинтс
description: Представляет платформы, предназначенные для уведомлений пользователей.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 9c1911900f4945d6f4b75d62c62457791fbb5c6a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939469"
---
# <a name="targetpolicyendpoints-resource-type"></a>Тип ресурса Таржетполициендпоинтс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет платформы, которые могут быть предназначены для получения уведомлений, отправляемых пользователю.  К ним относятся Windows, iOS, Android и веб-сайт. 


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|платформтипес|Коллекция строк|Используется для фильтрации распространения уведомлений на определенную платформу или платформы. Допустимые значения `Windows`: `iOS`, `Android` и `WebPush`. По умолчанию все типы конечных точек Push (Windows, iOS, Android и Push) включены. |

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