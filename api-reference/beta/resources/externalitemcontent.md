---
title: Тип ресурса externalItemContent
description: Содержимое элемента, индексироваться через подключение Поиска (Майкрософт).
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 66e3fccc8c072d06d2328301100d6bf3a0d50806
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777633"
---
# <a name="externalitemcontent-resource-type"></a>Тип ресурса externalItemContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержимое [externalItem, индексироваться](externalitem.md) через подключение Поиска (Майкрософт). [](externalconnection.md)

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| значение    | String | Содержимое для externalItem. Обязательное.                                                 |
| type     | String | Тип контента в свойстве value. Возможные значения: `text` и `html`. Обязательный. |

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


