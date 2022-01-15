---
title: Тип ресурса attachmentItem
description: Представляет атрибуты элемента, который необходимо прикрепить.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 219632b035b31a32428bd27aac324cb99dda168d
ms.sourcegitcommit: 94741ff7f61f20a39dacfa6ce451a77ca02dd68a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2022
ms.locfileid: "62047086"
---
# <a name="attachmentitem-resource-type"></a>Тип ресурса attachmentItem

Пространство имен: microsoft.graph

Представляет атрибуты элемента, который необходимо прикрепить.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|attachmentType|String| Тип вложения. Возможные значения: `file`, `item`, `reference`. Обязательное.|
|contentId|String| CiD или Content-Id вложения для ссылок в случае вложений в строке с помощью тега `<img src="cid:contentId">` в HTML-сообщениях. Необязательно.|
|contentType|String|Характер данных в приложении. Необязательно.|
|isInline|Boolean|Значение `true`, если вложение является встроенным. В противном случае — значение `false`. Необязательно.|
|name|String|Отображаемое имя вложения. Это может быть описательная строка и не должна быть фактическим именем файла. Обязательное.|
|size|Int64|Размер вложения в байтах. Обязательный элемент.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentId",
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
  "contentId": "String",
  "contentType": "String",
  "isInline": true,
  "name": "String",
  "size": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachmentItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
