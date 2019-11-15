---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 0bba7fce9557c6c249ea9aefced5a198a87f5026
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658809"
---
# <a name="itembody-resource-type"></a>Тип ресурса itemBody

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства основного текста элемента, например сообщения, события или записи группы.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|content|String|Содержимое элемента.|
|contentType|String|Тип контента. Возможные значения: `text` и `html`.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
