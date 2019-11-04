---
title: Тип ресурса Пайлоадтипес
description: Представляет данные уведомления о необработанном или визуальном пользователе, которое будет доставлено клиенту приложения, получающим это уведомление, и использоваться им.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 2d740c5b19b363fa2534984bf059cd186b065e89
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939609"
---
# <a name="payloadtypes-resource-type"></a>Тип ресурса Пайлоадтипес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот ресурс представляет данные о необработанном или визуальном уведомлении пользователя, которые будут доставлены и использованы клиентом приложения, получающим это уведомление.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|равконтент|Строка|Контент уведомления необработанного пользователя, который будет доставляться и потребляться клиентом приложения на всех поддерживаемых платформах (Windows, iOS, Android или The-Push), получающих это уведомление. По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.|
|висуалконтент|[висуалпропертиес](visualproperties.md)|Визуальное содержимое уведомления визуального пользователя, которое будет использоваться платформой уведомлений на каждой поддерживаемой платформе (только для Windows, iOS и Android) и визуализирована для пользователя. По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.payloadTypes",
  "baseType": null
}-->

```json
{
  "rawContent": "String",
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "payloadTypes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->