---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 036b2e2d4081160680b7f5471bd2707ee503bc4a
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366543"
---
# <a name="externalitemcontent-resource-type"></a>тип ресурса externalItemContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержимое [externalItem,](externalitem.md) индексироваться с помощью Поиск (Майкрософт) [подключения](externalconnection.md).

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| значение    | String | Содержимое для externalItem. Обязательное.                                                 |
| type     | String | Тип контента в свойстве значения. Возможные значения: `text` и `html`. Обязательный. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent"
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->


