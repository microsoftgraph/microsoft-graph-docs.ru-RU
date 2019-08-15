---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4cfa6fe84c18d4895e5d709d3ab6254258c1b970
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422284"
---
# <a name="patchcontentcommand-resource-type"></a>Тип ресурса Патчконтенткомманд

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [Patch Pages/{ID} '](../api/page-update.md) . 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|action|String|Действие, которое необходимо выполнить для целевого элемента. Возможные значения: `replace`, `append`, `delete`, `insert` и `prepend`.|
|content|String|Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если содержимое содержит двоичные данные, необходимо отправить запрос, используя тип `multipart/form-data` контента с частью "Commands". |
|position|String|Место для добавления предоставленного контента относительно целевого элемента. Возможные значения: `after` (по умолчанию) `before`или.|
|target|String|Обновляемый элемент. Должен быть `#<data-id>` либо сгенерированным `{id}` элементом, либо ключевым словом `body` or. `title`|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
