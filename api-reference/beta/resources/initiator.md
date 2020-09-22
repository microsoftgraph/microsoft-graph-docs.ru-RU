---
title: Тип ресурса инициатора
description: Указывает, кто инициировал событие подготовки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0b6b326925d0ca3f0dbf8c0c25df266834ecce6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021912"
---
# <a name="initiator-resource-type"></a>Тип ресурса инициатора

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, кто инициировал событие подготовки. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Имя пользователя или службы, которые инициировали событие подготовки.|
|id|String|Уникальный идентификатор пользователя или службы, которые инициировали событие подготовки.|
|инитиатортипе|String| Тип инициатора. Возможные значения: `user`, `app`, `system`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


