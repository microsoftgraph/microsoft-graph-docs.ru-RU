---
title: Тип ресурса инициатора
description: Указывает, кто инициировал событие подготовки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2846c247d4a0d196d4c620f447b40d47cd486c81
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349454"
---
# <a name="initiator-resource-type"></a>Тип ресурса инициатора

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, кто инициировал событие подготовки. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Имя пользователя или службы, которые инициировали событие подготовки.|
|id|String|Уникальный идентификатор пользователя или службы, которые инициировали событие подготовки.|
|Инитиатортипе|String| Тип инициатора. Возможные значения: `user`, `app`, `system`, `unknownFutureValue`.|

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
