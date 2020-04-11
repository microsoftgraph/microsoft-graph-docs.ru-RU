---
title: Тип ресурса Релатедперсон
description: Тип ресурса Релатедперсон
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c440be4ad291857fad9540cccad2e43d3a0e7121
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227706"
---
# <a name="relatedperson-resource-type"></a>Тип ресурса Релатедперсон

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о пользователях, связанных с информацией в данной сущности в [профиле](profile.md) пользователя.

## <a name="properties"></a>Свойства

| Свойство        | Тип        | Описание                                                                                                                                                                                                                                     |
|:----------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|displayName      |Строка       | Имя пользователя.                                                                                                                                                                                                                             |
|Отношение     |String       | Возможные значения: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.|
|userPrincipalName|String       | Адрес электронной почты или ссылка на пользователя в Организации.                                                                                                                                                                                       |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedPerson",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "relationship": "String",
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relatedPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
