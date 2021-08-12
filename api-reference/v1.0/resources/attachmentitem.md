---
title: Тип ресурса attachmentItem
description: Представляет атрибуты элемента, который необходимо прикрепить.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c50576b203254517d0718fc32d7322a42eb67b9160b848081f687fc35c0748a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182604"
---
# <a name="attachmentitem-resource-type"></a>Тип ресурса attachmentItem

Пространство имен: microsoft.graph

Представляет атрибуты элемента, который необходимо прикрепить.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|attachmentType|String| Тип вложения. Возможные значения: `file`, `item`, `reference`. Обязательное.|
|contentType|String|Характер данных в приложении. Необязательно.|
|isInline|Boolean|Значение `true`, если вложение является встроенным. В противном случае — значение `false`. Необязательно.|
|name|String|Отображаемое имя вложения. Это может быть описательная строка и не должна быть фактическим именем файла. Обязательный элемент.|
|size|Int64|Размер вложения в байтах. Обязательный элемент.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
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
